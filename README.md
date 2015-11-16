# Common Module Hooks for Beaver Builder Modules - Proposal [Draft]

This is a working draft proposal for a set of common module hooks for Beaver Builder module development. These hooks are designed to lessen the need to override built-in modules or create very similar custom modules.

## Hook Opportunities
* Module Element - allow semantic elements to be chosen on the wrapping element besides just a div.
* Module Class Names
* Module wrapper attributes
* Before module output
* After module output
* Additional filter: register_module forms
* 

## Example frontend.php
```php
<?php
<<?php module_element('div') ?> <?php module_class('my-module-class') ?>>
<?php before_module() ?>
  <div>
    <div>super cool module content</div>
  </div>
<?php after_module() ?>
</div>
?>
```
