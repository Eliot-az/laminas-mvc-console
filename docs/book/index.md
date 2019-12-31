> ### Deprecated!
> 
> Due to the amount of integration required to support console tooling via the
> MVC, and because [better, more standalone solutions
> exist](https://github.com/zfcampus/zf-console), **we will not be maintaining
> laminas-mvc-console long term**. We strongly urge developers to start migrating their
> MVC-based console tooling to use other libraries, such as
> [zf-console](https://github.com/zfcampus/zf-console).

---

> ### For use with laminas-mvc v3 and up
> 
> While this component has an initial stable release, please do not use it with
> laminas-mvc releases prior to v3, as it is not compatible.

## Installation

```console
$ composer require laminas/laminas-mvc-console
```

Assuming you are using the [component
installer](https://docs.laminas.dev/laminas-component-installer), doing so
will enable the component in your application, allowing you to immediately start
developing console applications via your MVC.

> ### Manual installation
>
> If you are not using the component installer, you will need to add this
> component as a module at the start of your module list in your Laminas
> application.
>
> If using a vanilla skeleton application, update `config/application.config.php`:
>
> ```php
> 'modules' => [
>     'Laminas\Mvc\Console', // add it to the top of your module list
>     /* ... */
> ]
> ```
>
> If using Laminas API Tools, update your `config/modules.config.php`:
>
> ```php
> return [
>     'Laminas\Mvc\Console', // add it to the top of your module list
>     /* ... */
> ];
> ```

## Migration
 
In order to separate the console tooling from laminas-mvc and provide it as a
standalone package, we needed to make a few changes. See the
[migration guide](migration/v2-to-v3.md) for details.
