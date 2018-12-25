## Accordion

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Accordion w/ Default</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'            => 'opt-accordion-1',
  'type'          => 'accordion',
  'title'         => 'Accordion',
  'accordions'    => array(
    array(
      'title'     => 'Accordion 1',
      'icon'      => 'fa fa-heart',
      'fields'    => array(
        array(
          'id'    => 'opt-text-1',
          'type'  => 'text',
          'title' => 'Text',
        ),
      )
    ),
    array(
      'title'     => 'Accordion 2',
      'icon'      => 'fa fa-gear',
      'fields'    => array(
        array(
          'id'    => 'opt-color-1',
          'type'  => 'color',
          'title' => 'Color',
        ),
      )
    ),
  )
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'            => 'opt-accordion-2',
  'type'          => 'accordion',
  'title'         => 'Accordion',
  'accordions'    => array(
    array(
      'title'     => 'Accordion 1',
      'icon'      => 'fa fa-heart',
      'fields'    => array(
        array(
          'id'    => 'opt-text-1',
          'type'  => 'text',
          'title' => 'Text 1',
        ),
        array(
          'id'    => 'opt-text-2',
          'type'  => 'text',
          'title' => 'Text 2',
        ),
      )
    ),
    array(
      'title'     => 'Accordion 2',
      'fields'    => array(
        array(
          'id'    => 'opt-color-1',
          'type'  => 'color',
          'title' => 'Color 1',
        ),
        array(
          'id'    => 'opt-color-2',
          'type'  => 'color',
          'title' => 'Color 2',
        ),
      )
    ),
  ),
  'default'       => array(
    'opt-text-1'  => 'This is text 1 value',
    'opt-text-2'  => 'This is text 2 value',
    'opt-color-1' => '#555',
    'opt-color-2' => '#999',
  ),
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type         | Default    | Description |
|------------------|--------------|------------|-------------|
| `id`             | string       |            | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string       | accordion  | The type of the field.
| `title`          | string       |            | The title of the field.
| `default`        | array        |            | The default value to return if the option does not exist in the database
| `subtitle`       | string       |            | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string       |            | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string       |            | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string       |            | The extra CSS classes (space separated) to append to the field.
| `before`         | string       |            | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string       |            | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array        |            | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array        |            | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string       |            | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string       |            | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---          | ---        | ---
| `accordions`     | array        |            | An associative array containing fields for the fieldsets.

----------------------------------------------------------------------------------------------------------------------------------------------

## Background

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Advanced</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-background-1',
  'type'  => 'background',
  'title' => 'Background',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'                              => 'opt-background-2',
  'type'                            => 'background',
  'title'                           => 'Background',
  'background_gradient'             => true,
  'background_origin'               => true,
  'background_clip'                 => true,
  'background_blend-mode'           => true,
  'default'                         => array(
    'background-color'              => '#111',
    'background-gradient-color'     => '#555',
    'background-gradient-direction' => 'to bottom',
    'background-size'               => 'cover',
    'background-position'           => 'center center',
    'background-repeat'             => 'repeat',
  )
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name                       | Type          | Default     | Description |
|----------------------------|---------------|-------------|-------------|
| `id`                       | string        |             | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`                     | string        | background  | The type of the field.
| `title`                    | string        |             | The title of the field.
| `default`                  | array         |             | The default value to return if the option does not exist in the database
| `subtitle`                 | string        |             | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`                     | string        |             | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`                     | string        |             | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`                    | string        |             | The extra CSS classes (space separated) to append to the field.
| `before`                   | string        |             | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`                    | string        |             | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`               | array         |             | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`               | array         |             | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`                 | string        |             | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`                 | string        |             | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**                 | ---           | ---         | ---
| `background_color`         | bool          | true        | Whether to show *background color* of the field.
| `background_image`         | bool          | true        | Whether to show *background image* of the field.
| `background_position`      | bool          | true        | Whether to show *background position* of the field.
| `background_repeat`        | bool          | true        | Whether to show *background repeat* of the field.
| `background_attachment`    | bool          | true        | Whether to show *background attachment* of the field.
| `background_size`          | bool          | true        | Whether to show *background size* of the field.
| `background_origin`        | bool          | false       | Whether to show *background origin* of the field.
| `background_clip`          | bool          | false       | Whether to show *background clip* of the field.
| `background_blend_mode`    | bool          | false       | Whether to show *background blend mode* of the field.
| `background_gradient`      | bool          | false       | Whether to show *background gradient* of the field.
| `background_image_preview` | bool          | true        | Whether to show *background image preview* of the field.
| `output`                   | array\|string |             | The CSS elements selector.
| `output_important`         | bool          | false       | Whether to add **!important** rule on output css

<div class="pre-heading">Default Arguments</div>

| Name                            | Type       | Description |
|---------------------------------|------------|-------------|
| `background-color`              | string     | A validated color value. *for eg.* `#ffbc00`, `rgba(255,0,0,0.25)`
| `background-position`           | string     | A defined value. *for eg.* `left top` `left center` `left bottom`<br /> `center top` `center center` `center bottom`<br /> `right top` `right center` `right bottom`
| `background-repeat`             | string     | A defined value. *for eg.* `repeat` `repeat-x` `repeat-y` `no-repeat`
| `background-attachment`         | string     | A defined value. *for eg.* `scroll` `fixed`
| `background-size`               | string     | A defined value. *for eg.* `cover` `contain`
| `background-origin`             | string     | A defined value. *for eg.* `padding-box` `border-box` `content-box`
| `background-clip`               | string     | A defined value. *for eg.* `padding-box` `border-box` `content-box`
| `background-blend-mode`         | string     | A defined value. *for eg.* `normal` `multiply` `screen` `overlay` `darken`<br/> `lighten` `color-dodge` `saturation` `color` `luminosity`
| `background-gradient-color`     | string     | A defined value. *for eg.* `#ffbc00`, `rgba(255,0,0,0.25)`
| `background-gradient-direction` | string     | A defined value. *for eg.* `to bottom` `to right` `135deg` `-135deg`

----------------------------------------------------------------------------------------------------------------------------------------------

## Backup

<div class="pre-heading">Config Example</div>

```php
array(
  'type' => 'backup',
),
```

<div class="pre-heading">Arguments</div>

| Name        | Type    | Default  | Description |
|-------------|---------|----------|-------------|
| `type`      | string  | backup   | The type of the field.
| `title`     | string  |          | The title of the field.
| `subtitle`  | string  |          | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`      | string  |          | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`      | string  |          | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`     | string  |          | The extra CSS classes (space separated) to append to the field.
| `before`    | string  |          | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`     | string  |          | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>

----------------------------------------------------------------------------------------------------------------------------------------------

## Border

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Border w/ Default</span>
<span class="csf-tab-title">Border w/ Join Borders</span>
<span class="csf-tab-title">Border w/ Spesific</span>
<span class="csf-tab-title">Border w/ Output</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'     => 'opt-border-1',
  'type'   => 'border',
  'title'  => 'Border',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-border-2',
  'type'    => 'border',
  'title'   => 'Border',
  'default' => array(
    'top'    => '4',
    'right'  => '8',
    'bottom' => '4',
    'left'   => '8',
    'style'  => 'dashed',
    'color'  => '#1e73be',
    'unit'          => 'px',
  ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'    => 'opt-border-3',
  'type'  => 'border',
  'title' => 'Border',
  'all'   => true,
),
```
</div>
<div class="csf-tab-content">

```php
// Without top and bottom borders
array(
  'id'     => 'opt-border-4',
  'type'   => 'border',
  'title'  => 'Border',
  'top'    => false,
  'bottom' => false,
),

// Without left and right borders
array(
  'id'    => 'opt-border-5',
  'type'  => 'border',
  'title' => 'Border',
  'left'  => false,
  'right' => false,
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'     => 'opt-border-6',
  'type'   => 'border',
  'title'  => 'Border',
  'output' => '.heading'
),

array(
  'id'     => 'opt-border-7',
  'type'   => 'border',
  'title'  => 'Border',
  'output' => array( '.header-area', '.footer-area' ),
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name                | Type           | Default      | Description |
|---------------------|----------------|--------------|-------------|
| `id`                | string         |              | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`              | string         | border       | The type of the field.
| `title`             | string         |              | The title of the field.
| `default`           | array          |              | The default value to return if the option does not exist in the database
| `subtitle`          | string         |              | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`              | string         |              | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`              | string         |              | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`             | string         |              | The extra CSS classes (space separated) to append to the field.
| `before`            | string         |              | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`             | string         |              | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`        | array          |              | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`        | array          |              | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`          | string         |              | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`          | string         |              | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**          | ---            | ---          | ---
| `top_icon`          | string         | top-icon     | The icon/text to display on the *top* field.
| `right_icon`        | string         | right-icon   | The icon/text to display on the *right* field.
| `bottom_icon`       | string         | bottom-icon  | The icon/text to display on the *bottom* field.
| `left_icon`         | string         | left-icon    | The icon/text to display on the *left* field.
| `all_icon`          | string         | all-icon     | The icon/text to display on the *all corners* field.
| `top`               | bool           | true         | Whether to show *top* of the field.
| `right`             | bool           | true         | Whether to show *right* of the field.
| `bottom`            | bool           | true         | Whether to show *bottom* of the field.
| `left`              | bool           | true         | Whether to show *left* of the field.
| `color`             | bool           | true         | Whether to show *color* of the field.
| `style`             | bool           | true         | Whether to show *style* of the field.
| `all`               | bool           | false        | Whether to show *all corners* of the field.
| `unit`              | string         | px           | The unit to display on the border inputs, also sets output CSS property unit value.
| `output`            | array\|string  |              | The CSS elements selector.
| `output_important`  | bool           | false        | Whether to add **!important** rule on output CSS

<div class="pre-heading">Default Arguments</div>

| Name             | Type      | Description |
|------------------|-----------|-------------|
| `top`     | number    | A numeric value
| `right`   | number    | A numeric value
| `bottom`  | number    | A numeric value
| `left`    | number    | A numeric value
| `all`     | number    | A numeric value
| `color`   | string    | A validated color value. *for eg.* `#ffbc00`, `rgba(255,0,0,0.25)`
| `style`   | string    | A defined value. *for eg.* `solid` `dashed` `dotted` `double` `none`
| `unit`    | string    | A defined value. *for eg.* `px` `em` `%`

----------------------------------------------------------------------------------------------------------------------------------------------

## Button Set

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Multiple Options</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'         => 'opt-button-set-1',
  'type'       => 'button_set',
  'title'      => 'Button Set',
  'options'    => array(
    'enabled'  => 'Enabled',
    'disabled' => 'Disabled',
  ),
  'default'    => 'enabled'
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'       => 'opt-button-set-2',
  'type'     => 'button_set',
  'title'    => 'Button Set with multiple',
  'multiple' => true,
  'options'  => array(
    'aqua'   => 'Aqua',
    'cyan'   => 'Cyan',
    'golden' => 'Golden',
    'indigo' => 'Indigo',
    'lime'   => 'Lime',
    'navy'   => 'Navy',
    'purple' => 'Purple',
  ),
  'default'  => array( 'cyan', 'indigo', 'purple' )
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type           | Default     | Description |
|------------------|----------------|-------------|-------------|
| `id`             | string         |             | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string         | button_set  | The type of the field.
| `title`          | string         |             | The title of the field.
| `default`        | array\|string  |             | The default value to return if the option does not exist in the database
| `subtitle`       | string         |             | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string         |             | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string         |             | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string         |             | The extra CSS classes (space separated) to append to the field.
| `before`         | string         |             | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string         |             | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array          |             | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array          |             | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string         |             | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string         |             | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---            | ---         | ---
| `multiple`       | bool           | false       | Whether to allows multiple options choose.
| `options`        | array          |             | An array of object containing key/value pairs representing the options.

----------------------------------------------------------------------------------------------------------------------------------------------

## Checkbox

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Single Option</span>
<span class="csf-tab-title">Multiple Options</span>
<span class="csf-tab-title">WP Query Options</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'      => 'opt-checkbox-1',
  'type'    => 'checkbox',
  'title'   => 'Checkbox',
  'label'   => 'Yes, Please do it.',
  'default' => true // or false
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'         => 'opt-checkbox-2',
  'type'       => 'checkbox',
  'title'      => 'Checkboxes',
  'options'    => array(
    'option-1' => 'Option 1',
    'option-2' => 'Option 2',
    'option-3' => 'Option 3',
  ),
  'default'    => array( 'option-1', 'option-3' )
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'         => 'opt-checkbox-3',
  'type'       => 'checkbox',
  'title'      => 'Checkbox with Pages',
  'options'    => 'categories', // pages, posts, tags, menus
  'query_args' => array(
    'order'    => 'title',
    'orderby'  => 'name',
  ),
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type           | Default     | Description |
|------------------|----------------|-------------|-------------|
| `id`             | string         |             | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string         | checkbox    | The type of the field.
| `title`          | string         |             | The title of the field.
| `default`        | array\|string  |             | The default value to return if the option does not exist in the database
| `subtitle`       | string         |             | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string         |             | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string         |             | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string         |             | The extra CSS classes (space separated) to append to the field.
| `before`         | string         |             | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string         |             | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array          |             | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array          |             | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string         |             | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string         |             | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---            | ---         | ---
| `label`          | string         |             | The text to display with the checkbox, when use to single checkbox.
| `options`        | array\|string  |             | An array of object containing key/value pairs representing the options or use a predefined options. *for eg.* `pages` `posts` `menus`
| `query_args`     | array          |             | An associative array of query arguments.

----------------------------------------------------------------------------------------------------------------------------------------------

## Code Editor

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">HMTL Editor</span>
<span class="csf-tab-title">CSS Editor</span>
<span class="csf-tab-title">Javascript Editor</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-code-editor-1',
  'type'  => 'code_editor',
  'title' => 'Code Editor',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'       => 'opt-code-editor-2',
  'type'     => 'code_editor',
  'title'    => 'HTML Editor',
  'settings' => array(
    'theme'  => 'mdn-like',
    'mode'   => 'htmlmixed',
  ),
  'default'  => '<h1>Hello world</h1>',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'       => 'opt-code-editor-3',
  'type'     => 'code_editor',
  'title'    => 'CSS Editor',
  'settings' => array(
    'theme'  => 'mbo',
    'mode'   => 'css',
  ),
  'default'  => '.element{ color: #ffbc00; }',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'       => 'opt-code-editor-4',
  'type'     => 'code_editor',
  'title'    => 'Javascript Editor',
  'settings' => array(
    'theme'  => 'monokai',
    'mode'   => 'javascript',
  ),
  'default'  => 'console.log("Hello world");',
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type         | Default      | Description |
|------------------|--------------|--------------|-------------|
| `id`             | string       |              | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string       | code_editor  | The type of the field.
| `title`          | string       |              | The title of the field.
| `default`        | string       |              | The default value to return if the option does not exist in the database
| `subtitle`       | string       |              | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string       |              | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string       |              | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string       |              | The extra CSS classes (space separated) to append to the field.
| `before`         | string       |              | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string       |              | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array        |              | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array        |              | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string       |              | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string       |              | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---          | ---          | ---
| `settings`       | array        |              | An associative array containing arguments for the setting.

<div class="pre-heading">Settings Arguments</div>

| Name          | Type       | Default     | Description |
|---------------|------------|-------------|-------------|
| `mode`        | string     | htmlmixed   | Set a language modes. for eg. `css` `javascript` `php`
| `theme`       | string     | default     | Set a  theme to style the editor. for eg. `mbo` `monokai` `ambiance`
| `lineNumbers` | bool       | true        | Whether to show line numbers to the left of the editor.
| `tabSize`     | number     | 2           | The width of a tab character.

Get more informations for [codemirror arguments](https://codemirror.net/doc/manual.html#config)

----------------------------------------------------------------------------------------------------------------------------------------------

## Color

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Color w/ Default</span>
<span class="csf-tab-title">Color w/ Output</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-color-1',
  'type'  => 'color',
  'title' => 'Color',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-color-2',
  'type'    => 'color',
  'title'   => 'Color',
  'default' => '#ffbc00'
),
```
</div>
<div class="csf-tab-content">

```php
// Output Example 1
array(
  'id'     => 'opt-color-3',
  'type'   => 'color',
  'title'  => 'Color',
  'output' => '.element-1'
),

// Output Example 2
array(
  'id'     => 'opt-color-4',
  'type'   => 'color',
  'title'  => 'Color',
  'output' => array( '.element-1', '.element-2', '.element-3' )
),

// Output Example 3
array(
  'id'     => 'opt-color-5',
  'type'   => 'color',
  'title'  => 'Color',
  'output' => array( 'background-color' => '.element-1', '.element-2', '.element-3' )
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name                | Type           | Default  | Description |
|---------------------|----------------|----------|-------------|
| `id`                | string         |          | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`              | string         | color    | The type of the field.
| `title`             | string         |          | The title of the field.
| `default`           | string         |          | The default value to return if the option does not exist in the database
| `subtitle`          | string         |          | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`              | string         |          | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`              | string         |          | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`             | string         |          | The extra CSS classes (space separated) to append to the field.
| `before`            | string         |          | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`             | string         |          | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`        | array          |          | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`        | array          |          | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`          | string         |          | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`          | string         |          | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**          | ---            | ---      | ---
| `output`            | array\|string  |          | The CSS elements selector.
| `output_mode`       | string         |          | The output CSS property of an element. for eg. `background-color` `color` `border-color`
| `output_important`  | bool           | false    | Whether to add **!important** rule on output css

----------------------------------------------------------------------------------------------------------------------------------------------

## Color Group

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Color Group w/ Default</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'        => 'opt-color-group-1',
  'type'      => 'color',
  'title'     => 'Color',
  'options'   => array(
    'color-1' => 'Color 1',
    'color-2' => 'Color 2',
    'color-3' => 'Color 3',
  )
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'        => 'opt-color-group-2',
  'type'      => 'color',
  'title'     => 'Color',
  'options'   => array(
    'color-1' => 'Color 1',
    'color-2' => 'Color 2',
    'color-3' => 'Color 3',
  ),
  'default'   => array(
    'color-1' => '#ffce4b',
    'color-2' => '#ff595e',
    'color-3' => '#0052cc',
  )
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name               | Type     | Default      | Description |
|--------------------|----------|--------------|-------------|
| `id`               | string   |              | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`             | string   | color_group  | The type of the field.
| `title`            | string   |              | The title of the field.
| `default`          | array    |              | The default value to return if the option does not exist in the database
| `subtitle`         | string   |              | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`             | string   |              | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`             | string   |              | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`            | string   |              | The extra CSS classes (space separated) to append to the field.
| `before`           | string   |              | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`            | string   |              | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`       | array    |              | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`       | array    |              | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`         | string   |              | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`         | string   |              | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**         | ---      | ---          | ---
| `options`          | array    |              | An array of object containing key/value(color) pairs representing the options.

----------------------------------------------------------------------------------------------------------------------------------------------

## Date

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Advanced</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-date-1',
  'type'  => 'date',
  'title' => 'Date',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'       => 'opt-date-2',
  'type'     => 'date',
  'title'    => 'Date Advanced',
  'settings' => array(
    'format'          => 'mm/dd/yy'
    'changeMonth'     => true,
    'changeYear'      => true,
    'showWeek'        => true,
    'showButtonPanel' => true,
    'weekHeader'      => 'Week',
    'monthNamesShort' => array( 'January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December' ),
    'dayNamesMin'     => array( 'Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday' ),
  )
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type     | Default  | Description |
|------------------|----------|----------|-------------|
| `id`             | string   |          | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string   | date     | The type of the field.
| `title`          | string   |          | The title of the field.
| `default`        | string   |          | The default value to return if the option does not exist in the database
| `subtitle`       | string   |          | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string   |          | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string   |          | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string   |          | The extra CSS classes (space separated) to append to the field.
| `before`         | string   |          | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string   |          | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array    |          | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array    |          | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string   |          | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string   |          | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---      | ---      | ---
| `settings`       | array    |          | An associative array containing arguments for the setting.

<div class="pre-heading">Settings Arguments</div>

| Name               | Type       | Default     | Description |
|--------------------|------------|-------------|-------------|
| `dateFormat`       | string     | mm/dd/yy    | The format for parsed and displayed dates.
| `changeMonth`      | bool       | false       | Whether the month should be rendered as a dropdown instead of text.
| `changeYear`       | bool       | false       | Whether the year should be rendered as a dropdown instead of text.
| `showWeek`         | bool       | false       | When true, a column is added to show the week of the year.
| `showButtonPanel`  | bool       | false       | Whether to display a button pane underneath the calendar.
| `weekHeader`       | string     | Wk          | The text to display for the week of the year column heading.
| `monthNamesShort`  | array      |             | The list of abbreviated month names, as used in the month header on each datepicker and as requested via the dateFormat option.
| `dayNamesMin`      | array      |             | The list of minimised day names, starting from Sunday, for use as column headers within the datepicker.

Get more informations for [jquery-ui-datepicker arguments](http://api.jqueryui.com/datepicker/#options)

----------------------------------------------------------------------------------------------------------------------------------------------

## Dimensions

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Dimensions w/ Default</span>
<span class="csf-tab-title">Dimensions w/ Output</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'     => 'opt-dimensions-1',
  'type'   => 'dimensions',
  'title'  => 'Dimensions width and height',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'       => 'opt-dimensions-2',
  'type'     => 'dimensions',
  'title'    => 'Dimensions with default',
  'default'  => array(
    'width'  => '100',
    'height' => '250',
    'unit'   => 'px',
  ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'     => 'opt-dimensions-3',
  'type'   => 'dimensions',
  'title'  => 'Dimensions',
  'output' => '.heading'
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name                | Type           | Default      | Description |
|---------------------|----------------|--------------|-------------|
| `id`                | string         |              | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`              | string         | dimensions   | The type of the field.
| `title`             | string         |              | The title of the field.
| `default`           | array          |              | The default value to return if the option does not exist in the database
| `subtitle`          | string         |              | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`              | string         |              | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`              | string         |              | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`             | string         |              | The extra CSS classes (space separated) to append to the field.
| `before`            | string         |              | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`             | string         |              | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`        | array          |              | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`        | array          |              | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`          | string         |              | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`          | string         |              | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**          | ---            | ---          | ---
| `width_icon`        | string         | width-icon   | The icon/text to display on the *width* of the field.
| `height_icon`       | string         | height-icon  | The icon/text to display on the *height* of the field.
| `width`             | bool           | true         | Whether to show *width* of the field.
| `height`            | bool           | true         | Whether to show *height* of the field.
| `unit`              | bool           | true         | Whether to show *unit selector* of the field.
| `units`             | array          |              | The CSS measurement units, *for eg.* `px` `em` `%` `cm` `pt`
| `output`            | array\|string  |              | The CSS elements selector.
| `output_prefix`     | string         |              | The setting for add `max` / `min` to output CSS property of element. *for eg.* `max-width` `max-height`
| `output_important`  | bool           | false        | Whether to add **!important** rule on output css

<div class="pre-heading">Default Arguments</div>

| Name      | Type      | Description |
|-----------|-----------|-------------|
| `width`   | number    | A numeric value
| `height`  | number    | A numeric value
| `unit`    | string    | A defined value. *for eg.* `px` `em` `%`

----------------------------------------------------------------------------------------------------------------------------------------------

## Fieldset

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Fieldset w/ Default</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'     => 'opt-fieldset-1',
  'type'   => 'fieldset',
  'title'  => 'Fieldset',
  'fields' => array(
    array(
      'id'    => 'opt-text',
      'type'  => 'text',
      'title' => 'Text',
    ),
    array(
      'id'    => 'opt-color',
      'type'  => 'color',
      'title' => 'Color',
    ),
    array(
      'id'    => 'opt-switcher',
      'type'  => 'switcher',
      'title' => 'Switcher',
    ),
  ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'        => 'opt-fieldset-2',
  'type'      => 'fieldset',
  'title'     => 'Fieldset',
  'fields'    => array(
    array(
      'id'    => 'opt-text',
      'type'  => 'text',
      'title' => 'Text',
    ),
    array(
      'id'    => 'opt-color',
      'type'  => 'color',
      'title' => 'Color',
    ),
    array(
      'id'    => 'opt-switcher',
      'type'  => 'switcher',
      'title' => 'Switcher',
    ),
  ),
  'default'        => array(
    'opt-text'     => 'Text default value',
    'opt-color'    => '#ffbc00',
    'opt-switcher' => true,
  ),
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type         | Default     | Description |
|------------------|--------------|-------------|-------------|
| `id`             | string       |             | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string       | fieldset    | The type of the field.
| `title`          | string       |             | The title of the field.
| `default`        | array        |             | The default value to return if the option does not exist in the database
| `subtitle`       | string       |             | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string       |             | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string       |             | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string       |             | The extra CSS classes (space separated) to append to the field.
| `before`         | string       |             | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string       |             | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array        |             | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array        |             | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string       |             | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string       |             | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---          | ---         | ---
| `fields`         | array        |             | An associative array containing fields for the fieldsets.

----------------------------------------------------------------------------------------------------------------------------------------------

## Gallery

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Gallery w/ Custom Title</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-gallery-1',
  'type'  => 'gallery',
  'title' => 'Gallery',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'          => 'opt-gallery-2',
  'type'        => 'gallery',
  'title'       => 'Gallery',
  'add_title'   => 'Add Images',
  'edit_title'  => 'Edit Images',
  'clear_title' => 'Remove Images',
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type         | Default        | Description |
|------------------|--------------|----------------|-------------|
| `id`             | string       |                | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string       | gallery        | The type of the field.
| `title`          | string       |                | The title of the field.
| `default`        | string       |                | The default value to return if the option does not exist in the database
| `subtitle`       | string       |                | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string       |                | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string       |                | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string       |                | The extra CSS classes (space separated) to append to the field.
| `before`         | string       |                | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string       |                | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array        |                | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array        |                | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string       |                | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string       |                | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---          | ---            | ---
| `add_title`      | string       | Add Gallery    | The text to display on the add button.
| `edit_title`     | string       | Edit Gallery   | The text to display on the edit button.
| `clear_title`    | string       | Clear          | The text to display on the clear button.

----------------------------------------------------------------------------------------------------------------------------------------------

## Group

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Group w/ Default</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'        => 'opt-group-1',
  'type'      => 'group',
  'title'     => 'Group',
  'fields'    => array(
    array(
      'id'    => 'opt-text',
      'type'  => 'text',
      'title' => 'Text',
    ),
    array(
      'id'    => 'opt-color',
      'type'  => 'color',
      'title' => 'Color',
    ),
    array(
      'id'    => 'opt-switcher',
      'type'  => 'switcher',
      'title' => 'Switcher',
    ),
  ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'        => 'opt-group-2',
  'type'      => 'group',
  'title'     => 'Group',
  'fields'    => array(
    array(
      'id'    => 'opt-text',
      'type'  => 'text',
      'title' => 'Text',
    ),
    array(
      'id'    => 'opt-color',
      'type'  => 'color',
      'title' => 'Color',
    ),
    array(
      'id'    => 'opt-switcher',
      'type'  => 'switcher',
      'title' => 'Switcher',
    ),
  ),
  'default'   => array(
    array(
      'opt-text'     => 'This is text default 1',
      'opt-color'    => '#ffbc00',
      'opt-switcher' => true,
    ),
    array(
      'opt-text'     => 'This is text default 2',
      'opt-color'    => '#000',
      'opt-switcher' => false,
    ),
  ),
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name                      | Type         | Default    | Description |
|---------------------------|--------------|------------|-------------|
| `id`                      | string       |            | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`                    | string       | group      | The type of the field.
| `title`                   | string       |            | The title of the field.
| `default`                 | array        |            | The default value to return if the option does not exist in the database
| `subtitle`                | string       |            | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`                    | string       |            | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`                    | string       |            | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`                   | string       |            | The extra CSS classes (space separated) to append to the field.
| `before`                  | string       |            | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`                   | string       |            | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`              | array        |            | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`              | array        |            | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`                | string       |            | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`                | string       |            | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**                | ---          | ---        | ---
| `fields`                  | array        |            | An associative array containing fields for the fieldsets.
| `max`                     | number       | 0          | The maximum number of items the user can add.
| `min`                     | number       | 0          | The minimum number of items the user can add.
| `button_title`            | string       | Add New    | The text to display on the add button.
| `remove_title`            | string       | Remove     | The text to display on the remove button.
| `accordion_title_prefix`  | string       |            | The text to display always on the pre title.
| `accordion_title_count`   | bool         | false      | The a counter to display on the pre title always. *for eg.* `1- Title` `2- Title`

----------------------------------------------------------------------------------------------------------------------------------------------

## Icon

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Icon w/ Default</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-icon-1',
  'type'  => 'icon',
  'title' => 'Icon',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-icon-2',
  'type'    => 'icon',
  'title'   => 'Icon',
  'default' => 'fa fa-heart'
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type         | Default      | Description |
|------------------|--------------|--------------|-------------|
| `id`             | string       |              | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string       | icon         | The type of the field.
| `title`          | string       |              | The title of the field.
| `default`        | string       |              | The default value to return if the option does not exist in the database
| `subtitle`       | string       |              | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string       |              | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string       |              | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string       |              | The extra CSS classes (space separated) to append to the field.
| `before`         | string       |              | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string       |              | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array        |              | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array        |              | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string       |              | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string       |              | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---          | ---          | ---
| `button_title`   | string       | Add Icon     | The text to display on the add button.
| `remove_title`   | string       | Remove Icon  | The text to display on the remove button.

----------------------------------------------------------------------------------------------------------------------------------------------

## Image Select

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Multiple w/ Default</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'        => 'opt-image-select-1',
  'type'      => 'image_select',
  'title'     => 'Image Select',
  'options'   => array(
    'value-1' => 'http://codestarframework.com/assets/images/placeholder/80x80-2c3e50.gif',
    'value-2' => 'http://codestarframework.com/assets/images/placeholder/80x80-2c3e50.gif',
    'value-3' => 'http://codestarframework.com/assets/images/placeholder/80x80-2c3e50.gif',
  ),
  'default'   => 'value-2'
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'        => 'opt-image-select-2',
  'type'      => 'image_select',
  'title'     => 'Image Select',
  'multiple'  => true,
  'options'   => array(
    'value-1' => 'http://codestarframework.com/assets/images/placeholder/80x80-2c3e50.gif',
    'value-2' => 'http://codestarframework.com/assets/images/placeholder/80x80-2c3e50.gif',
    'value-3' => 'http://codestarframework.com/assets/images/placeholder/80x80-2c3e50.gif',
  ),
  'default'   => array( 'value-1', 'value-3' )
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name                | Type           | Default       | Description |
|---------------------|----------------|---------------|-------------|
| `id`                | string         |               | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`              | string         | image_select  | The type of the field.
| `title`             | string         |               | The title of the field.
| `default`           | array\|string  |               | The default value to return if the option does not exist in the database
| `subtitle`          | string         |               | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`              | string         |               | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`              | string         |               | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`             | string         |               | The extra CSS classes (space separated) to append to the field.
| `before`            | string         |               | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`             | string         |               | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`        | array          |               | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`        | array          |               | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`          | string         |               | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`          | string         |               | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**          | ---            | ---           | ---
| `options`           | array          |               | An array of object containing key/value pairs representing the options.
| `multiple`          | bool           | false         | Whether to allows multiple options choose.
| `output`            | array\|string  |               | The CSS elements selector.
| `output_important`  | bool           | false         | Whether to add **!important** rule on output css

----------------------------------------------------------------------------------------------------------------------------------------------

## Link Color

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Link Color w/ Default</span>
<span class="csf-tab-title">Link Color w/ All</span>
<span class="csf-tab-title">Link Color w/ Output</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-link-color-1',
  'type'  => 'link_color',
  'title' => 'Link Color',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-link-color-2',
  'type'    => 'link_color',
  'title'   => 'Link Color',
  'default' => array(
    'color' => '#1e73be',
    'hover' => '#259ded',
  ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'        => 'opt-link-color-3',
  'type'      => 'link_color',
  'title'     => 'Link Color',
  'color'     => true,
  'hover'     => true,
  'visited'   => true,
  'active'    => true,
  'focus'     => true,
  'default'   => array(
    'color'   => '#1e73be',
    'hover'   => '#259ded',
    'visited' => '#222',
    'active'  => '#333',
    'focus'   => '#111',
  ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-link-color-4',
  'type'    => 'link_color',
  'title'   => 'Link Color',
  'output'  => '.heading',
  'default' => array(
    'color' => '#1e73be',
    'hover' => '#259ded',
  ),
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name               | Type           | Default      | Description |
|--------------------|----------------|--------------|-------------|
| `id`               | string         |              | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`             | string         | link_color   | The type of the field.
| `title`            | string         |              | The title of the field.
| `default`          | array          |              | The default value to return if the option does not exist in the database
| `subtitle`         | string         |              | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`             | string         |              | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`             | string         |              | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`            | string         |              | The extra CSS classes (space separated) to append to the field.
| `before`           | string         |              | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`            | string         |              | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`       | array          |              | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`       | array          |              | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`         | string         |              | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`         | string         |              | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**         | ---            | ---          | ---
| `color`            | bool           | true         | Whether to show *color* of the field. (normal, unvisited link)
| `hover`            | bool           | true         | Whether to show *hover* of the field. (link when the user mouses over it)
| `visited`          | bool           | false        | Whether to show *visited* of the field. (link the user has visited)
| `active`           | bool           | false        | Whether to show *active* of the field. (link the moment it is clicked)
| `focus`            | bool           | false        | Whether to show *focus* of the field. (link the focus)
| `output`           | array\|string  |              | The CSS elements selector.
| `output_important` | bool           | false        | Whether to add **!important** rule on output css

<div class="pre-heading">Default Arguments</div>

| Name      | Type    | Description |
|-----------|---------|-------------|
| `color`   | string  | A validated color value. *for eg.* `#1e73be`, `rgba(255,0,0,0.25)`
| `hover`   | string  | A validated color value. *for eg.* `#259ded`, `rgba(165,125,0,0.25)`
| `visited` | string  | A validated color value. *for eg.* `#2980b9`, `rgba(128,128,0,0.25)`
| `active`  | string  | A validated color value. *for eg.* `#d35400`, `rgba(152,55,25,0.25)`
| `focus`   | string  | A validated color value. *for eg.* `#2c3e50`, `rgba(55,100,150,0.25)`

----------------------------------------------------------------------------------------------------------------------------------------------

## Media

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Media without Preview</span>
<span class="csf-tab-title">Media only Image Formats</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-media-1',
  'type'  => 'media',
  'title' => 'Media',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-media-2',
  'type'    => 'media',
  'title'   => 'Media',
  'preview' => false,
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-media-3',
  'type'    => 'media',
  'title'   => 'Media',
  'library' => 'image',
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name              | Type           | Default           | Description |
|-------------------|----------------|-------------------|-------------|
| `id`              | string         |                   | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`            | string         | media             | The type of the field.
| `title`           | string         |                   | The title of the field.
| `default`         | array          |                   | The default value to return if the option does not exist in the database
| `subtitle`        | string         |                   | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`            | string         |                   | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`            | string         |                   | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`           | string         |                   | The extra CSS classes (space separated) to append to the field.
| `before`          | string         |                   | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`           | string         |                   | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`      | array          |                   | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`      | array          |                   | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`        | string         |                   | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`        | string         |                   | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**        | ---            | ---               | ---
| `url`             | bool           | true              | Whether to show *url* of the field.
| `preview`         | bool           | true              | Whether to show *preview* of the field.
| `library`         | array\|string  | all               | Tell the modal to show specific formats. for eg. `image` or `video` or both etc.
| `placeholder`     | string         | No media selected | The placeholder to be displayed when nothing is selected.
| `preview_size`    | string         | thumbnail         | The image size to use in preview. `thumbnail` or `full`
| `button_title`    | string         | Upload            | The text to display on the upload button.
| `remove_title`    | string         | Remove            | The text to display on the remove button.

<div class="pre-heading">Default Arguments</div>

| Name           | Type    | Description |
|----------------|---------|-------------|
| `url`          | string  | The url of the attachment
| `id`           | number  | The id of the attachment
| `width`        | number  | The width of the attachment
| `height`       | number  | The height of the attachment
| `thumbnail`    | string  | The thumbnail of the attachment
| `alt`          | string  | The alternate text of the attachment
| `title`        | string  | The title of the attachment
| `description`  | string  | The description of the attachment

----------------------------------------------------------------------------------------------------------------------------------------------

## Palette

<div class="pre-heading">Config Examples</div>

```php
array(
  'id'      => 'opt-palette-1',
  'type'    => 'palette',
  'title'   => 'Palette',
  'options' => array(
    'set1'  => array( '#f04e36', '#f36e27', '#f3d430', '#ed1683' ),
    'set2'  => array( '#f9ca06', '#b5b546', '#2f4d48', '#212b2f' ),
    'set3'  => array( '#4153ab', '#6e86c7', '#211f27', '#d69762' ),
    'set4'  => array( '#162526', '#508486', '#C8C6CE', '#B45F1A' ),
    'set5'  => array( '#bbd5ff', '#ccab5e', '#fff55f', '#197c5d' ),
  ),
  'default' => 'set3',
),
```

<div class="pre-heading">Arguments</div>

| Name          | Type     | Default   | Description |
|---------------|----------|-----------|-------------|
| `id`          | string   |           | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`        | string   | palette   | The type of the field.
| `title`       | string   |           | The title of the field.
| `default`     | string   |           | The default value to return if the option does not exist in the database
| `subtitle`    | string   |           | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`        | string   |           | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`        | string   |           | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`       | string   |           | The extra CSS classes (space separated) to append to the field.
| `before`      | string   |           | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`       | string   |           | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`  | array    |           | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`  | array    |           | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`    | string   |           | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`    | string   |           | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**    | ---      | ---       | ---
| `options`     | array    |           | An array of object containing key/array(colors) pairs representing the options.

----------------------------------------------------------------------------------------------------------------------------------------------

## Radio

<div class="pre-heading">Config Example</div>

```php
array(
  'id'         => 'opt-radio',
  'type'       => 'radio',
  'title'      => 'Radio',
  'options'    => array(
    'option-1' => 'Option 1',
    'option-2' => 'Option 2',
    'option-3' => 'Option 3',
  ),
  'default'    => 'option-2'
```

<div class="pre-heading">Arguments</div>

| Name             | Type           | Default  | Description |
|------------------|----------------|----------|-------------|
| `id`             | string         |          | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string         | radio    | The type of the field.
| `title`          | string         |          | The title of the field.
| `default`        | string         |          | The default value to return if the option does not exist in the database
| `subtitle`       | string         |          | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string         |          | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string         |          | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string         |          | The extra CSS classes (space separated) to append to the field.
| `before`         | string         |          | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string         |          | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array          |          | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array          |          | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string         |          | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string         |          | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---            | ---      | ---
| `options`        | array\|string  |          | An array of object containing key/value pairs representing the options or use a predefined options. *for eg.* `pages` `posts` `menus`
| `query_args`     | array          |          | An associative array of query arguments.

----------------------------------------------------------------------------------------------------------------------------------------------

## Repeater

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Repeater w/ Default</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'     => 'opt-repeater-1',
  'type'   => 'repeater',
  'title'  => 'Repeater',
  'fields' => array(

    array(
      'id'    => 'opt-text',
      'type'  => 'text',
      'title' => 'Text'
    ),

  ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'        => 'opt-repeater-2',
  'type'      => 'repeater',
  'title'     => 'Repeater',
  'fields'    => array(

    array(
      'id'    => 'opt-text-1',
      'type'  => 'text',
      'title' => 'Text',
    ),

    array(
      'id'    => 'opt-text-2',
      'type'  => 'text',
      'title' => 'Text',
    ),

  ),
  'default'   => array(
    array(
      'opt-text-1' => 'Text 1 default value',
      'opt-text-2' => 'Text 2 default value',
    ),
    array(
      'opt-text-1' => 'Text 1 default value',
      'opt-text-2' => 'Text 2 default value',
    )
  )
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type     | Default   | Description |
|------------------|----------|-----------|-------------|
| `id`             | string   |           | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string   | repeater  | The type of the field.
| `title`          | string   |           | The title of the field.
| `default`        | array    |           | The default value to return if the option does not exist in the database
| `subtitle`       | string   |           | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string   |           | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string   |           | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string   |           | The extra CSS classes (space separated) to append to the field.
| `before`         | string   |           | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string   |           | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array    |           | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array    |           | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string   |           | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string   |           | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---      | ---       | ---
| `fields`         | array    |           | An associative array containing fields for the fieldsets.
| `max`            | number   | 0         | The maximum number of items the user can add.
| `min`            | number   | 0         | The minimum number of items the user can add.
| `button_title`   | string   | plus-icon | The text to display on the add button.

----------------------------------------------------------------------------------------------------------------------------------------------

## Select

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Select w/ Groups</span>
<span class="csf-tab-title">Select w/ Chosen</span>
<span class="csf-tab-title">Select w/ Multiple Chosen</span>
<span class="csf-tab-title">Select w/ WP Query</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'          => 'opt-select-1',
  'type'        => 'select',
  'title'       => 'Select',
  'placeholder' => 'Select an option',
  'options'     => array(
    'option-1'  => 'Option 1',
    'option-2'  => 'Option 2',
    'option-3'  => 'Option 3',
  ),
  'default'     => 'option-2'
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'            => 'opt-select-2',
  'type'          => 'select',
  'title'         => 'Select',
  'placeholder'   => 'Select an option',
  'options'       => array(
    'Group Title' => array(
      'option-1'  => 'Option 1',
      'option-2'  => 'Option 2',
      'option-3'  => 'Option 3',
    ),
    'Group Title' => array(
      'option-4'  => 'Option 4',
      'option-5'  => 'Option 5',
      'option-6'  => 'Option 6',
    ),
  ),
  'default'       => array( 'option-2', 'option-5' )
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'          => 'opt-select-3',
  'type'        => 'select',
  'title'       => 'Select',
  'chosen'      => true,
  'placeholder' => 'Select an option',
  'options'     => array(
    'option-1'  => 'Option 1',
    'option-2'  => 'Option 2',
    'option-3'  => 'Option 3',
    'option-4'  => 'Option 4',
    'option-5'  => 'Option 5',
    'option-6'  => 'Option 6',
  ),
  'default'     => 'option-3'
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'          => 'opt-select-4',
  'type'        => 'select',
  'title'       => 'Select',
  'multiple'    => true,
  'chosen'      => true,
  'placeholder' => 'Select an option',
  'options'     => array(
    'option-1'  => 'Option 1',
    'option-2'  => 'Option 2',
    'option-3'  => 'Option 3',
    'option-4'  => 'Option 4',
    'option-5'  => 'Option 5',
    'option-6'  => 'Option 6',
  ),
  'default'     => 'option-3'
),
```
</div>
<div class="csf-tab-content">

```php
// Select with pages
array(
  'id'          => 'opt-select-5',
  'type'        => 'select',
  'title'       => 'Select with pages',
  'placeholder' => 'Select a page',
  'options'     => 'pages',
),

// Select with posts
array(
  'id'          => 'opt-select-6',
  'type'        => 'select',
  'title'       => 'Select with posts',
  'placeholder' => 'Select a post',
  'options'     => 'posts',
),

// Select with categories
array(
  'id'          => 'opt-select-7',
  'type'        => 'select',
  'title'       => 'Select with categories',
  'placeholder' => 'Select a category',
  'options'     => 'categories',
),

// Select with menus
array(
  'id'          => 'opt-select-8',
  'type'        => 'select',
  'title'       => 'Select with menus',
  'placeholder' => 'Select a menu',
  'options'     => 'menus',
),

// Select with CPT (custom post type) pages
array(
  'id'          => 'opt-select-9',
  'type'        => 'select',
  'title'       => 'Selec with CPT (custom post type) pages',
  'placeholder' => 'Select a page',
  'options'     => 'post_types',
  'query_args'  => array(
    'post_type' => 'your_post_type_name',
  ),
),

// Select with CPT (custom post type) categories
array(
  'id'          => 'opt-select-10',
  'type'        => 'select',
  'title'       => 'Selec with CPT (custom post type) category',
  'placeholder' => 'Select a category',
  'options'     => 'categories',
  'query_args'  => array(
    'type'      => 'your_post_type_name',
    'taxonomy'  => 'your_taxonomy_name',
  ),
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type           | Default  | Description |
|------------------|----------------|----------|-------------|
| `id`             | string         |          | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string         | select   | The type of the field.
| `title`          | string         |          | The title of the field.
| `default`        | array\|string  |          | The default value to return if the option does not exist in the database
| `subtitle`       | string         |          | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string         |          | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string         |          | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string         |          | The extra CSS classes (space separated) to append to the field.
| `before`         | string         |          | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string         |          | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array          |          | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array          |          | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string         |          | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string         |          | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---            | ---      | ---
| `placeholder`    | string         |          | The placeholder to be displayed when nothing is selected.
| `chosen`         | bool           | false    | Whether to enable [ChosenJS](https://harvesthq.github.io/chosen/) style select.
| `multiple`       | bool           | false    | Whether to allows multiple options choose.
| `options`        | array\|string  |          | An array of object containing key/value pairs representing the options or use a predefined options. *for eg.* `pages` `posts` `menus`
| `query_args`     | array          |          | An associative array of query arguments.

----------------------------------------------------------------------------------------------------------------------------------------------

## Slider

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Slider w/ Default</span>
<span class="csf-tab-title">Switcher w/ Max-Min</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-slider-1',
  'type'  => 'slider',
  'title' => 'Slider',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-slider-2',
  'type'    => 'slider',
  'title'   => 'Slider',
  'default' => 50,
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-slider-3',
  'type'    => 'slider',
  'title'   => 'Slider',
  'min'     => 0,
  'max'     => 100,
  'step'    => 1,
  'unit'    => 'px',
  'default' => 25,
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name                | Type           | Default  | Description |
|---------------------|----------------|----------|-------------|
| `id`                | string         |          | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`              | string         | slider   | The type of the field.
| `title`             | string         |          | The title of the field.
| `default`           | string         |          | The default value to return if the option does not exist in the database
| `subtitle`          | string         |          | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`              | string         |          | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`              | string         |          | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`             | string         |          | The extra CSS classes (space separated) to append to the field.
| `before`            | string         |          | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`             | string         |          | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`        | array          |          | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`        | array          |          | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`          | string         |          | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`          | string         |          | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**          | ---            | ---      | ---
| `max`               | number         | 100      | The maximum allowed value.
| `min`               | number         | 0        | The minimum allowed value.
| `step`              | number         | 1        | Amount of increment value for each step.
| `unit`              | string         | px       | The unit to display of the field, also sets output CSS property unit value.
| `output`            | array\|string  |          | The CSS elements selector.
| `output_mode`       | string         |          | The output CSS property of an element. for eg. `width` `height` `max-width` etc.
| `output_important`  | bool           | false    | Whether to add **!important** rule on output css

----------------------------------------------------------------------------------------------------------------------------------------------

## Sortable

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Sortable w/ Default</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'        => 'opt-sportable-1',
  'type'      => 'sortable',
  'title'     => 'Sortable',
  'fields'    => array(

    array(
      'id'    => 'text-1',
      'type'  => 'text',
      'title' => 'Text 1'
    ),

    array(
      'id'    => 'text-2',
      'type'  => 'text',
      'title' => 'Text 2'
    ),

  ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'        => 'opt-sportable-2',
  'type'      => 'sortable',
  'title'     => 'Sortable',
  'fields'    => array(

    array(
      'id'    => 'opt-text-1',
      'type'  => 'text',
      'title' => 'Text 1'
    ),

    array(
      'id'    => 'opt-text-2',
      'type'  => 'text',
      'title' => 'Text 2'
    ),

    array(
      'id'    => 'opt-text-3',
      'type'  => 'text',
      'title' => 'Text 3'
    ),

  ),
  'default'      => array(
    'opt-text-1' => 'This is text 1 default',
    'opt-text-2' => 'This is text 2 default',
    'opt-text-3' => 'This is text 3 default',
  ),
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type         | Default   | Description |
|------------------|--------------|-----------|-------------|
| `id`             | string       |           | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string       | sortable  | The type of the field.
| `title`          | string       |           | The title of the field.
| `default`        | array        |           | The default value to return if the option does not exist in the database
| `subtitle`       | string       |           | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string       |           | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string       |           | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string       |           | The extra CSS classes (space separated) to append to the field.
| `before`         | string       |           | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string       |           | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array        |           | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array        |           | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string       |           | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string       |           | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---          | ---       | ---
| `fields`         | array        |           | An associative array containing fields for the fieldsets.

----------------------------------------------------------------------------------------------------------------------------------------------

## Sorter

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Sorter w/ Custom Title</span>
<span class="csf-tab-title">Sorter without "Disabled"</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'           => 'opt-sorter-1',
  'type'         => 'sorter',
  'title'        => 'Sorter',
  'default'      => array(
    'enabled'    => array(
      'option-1' => 'Option 1',
      'option-2' => 'Option 2',
      'option-3' => 'Option 3',
    ),
    'disabled'   => array(
      'option-4' => 'Option 4',
      'option-5' => 'Option 5',
    ),
  ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'             => 'opt-sorter-2',
  'type'           => 'sorter',
  'title'          => 'Sorter',
  'default'        => array(
    'enabled'      => array(
      'option-1'   => 'Option 1',
      'option-2'   => 'Option 2',
      'option-3'   => 'Option 3',
    ),
    'disabled'     => array(
      'option-4'   => 'Option 4',
      'option-5'   => 'Option 5',
    ),
  ),
  'enabled_title'  => 'Activated',
  'disabled_title' => 'Deativated',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'           => 'opt-sorter-3',
  'type'         => 'sorter',
  'title'        => 'Sorter',
  'disabled'     => false,
  'default'      => array(
    'enabled'    => array(
      'option-1' => 'Option 1',
      'option-2' => 'Option 2',
      'option-3' => 'Option 3',
    ),
  ),
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name             | Type         | Default   | Description |
|------------------|--------------|-----------|-------------|
| `id`             | string       |           | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`           | string       | sorter    | The type of the field.
| `title`          | string       |           | The title of the field.
| `default`        | array        |           | The default value to return if the option does not exist in the database
| `subtitle`       | string       |           | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`           | string       |           | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`           | string       |           | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`          | string       |           | The extra CSS classes (space separated) to append to the field.
| `before`         | string       |           | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`          | string       |           | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`     | array        |           | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`     | array        |           | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`       | string       |           | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`       | string       |           | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**       | ---          | ---       | ---
| `disabled`       | bool         | true      | Whether to show *disabled items* of the field.
| `enabled_title`  | bool\|string | Enabled   | The text to display title of *Enabled* items. Set to *false* if want to hide title.
| `disabled_title` | bool\|string | Disabled  | The text to display title of *Disabled* items. Set to *false* if want to hide title.

----------------------------------------------------------------------------------------------------------------------------------------------

## Spacing

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Spacing w/ Default</span>
<span class="csf-tab-title">Spacing w/ Spesific</span>
<span class="csf-tab-title">Spacing w/ Output</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-spacing-1',
  'type'  => 'spacing',
  'title' => 'Spacing',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'       => 'opt-spacing-2',
  'type'     => 'spacing',
  'title'    => 'Spacing',
  'default'  => array(
    'top'    => '50',
    'right'  => '100',
    'bottom' => '50',
    'left'   => '100',
    'unit'   => 'px',
  ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'    => 'opt-spacing-3',
  'type'  => 'spacing',
  'title' => 'Spacing',
  'left'  => false,
  'right' => false,
  'units' => array( 'px' ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'          => 'opt-spacing-4',
  'type'        => 'spacing',
  'title'       => 'Spacing',
  'output'      => '.heading',
  'output_mode' => 'padding', // or margin, relative
  'default'     => array(
    'top'       => '10',
    'right'     => '20',
    'bottom'    => '10',
    'left'      => '20',
    'unit'      => 'px',
  ),
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name                | Type           | Default      | Description |
|---------------------|----------------|--------------|-------------|
| `id`                | string         |              | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`              | string         | spacing      | The type of the field.
| `title`             | string         |              | The title of the field.
| `default`           | array          |              | The default value to return if the option does not exist in the database
| `subtitle`          | string         |              | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`              | string         |              | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`              | string         |              | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`             | string         |              | The extra CSS classes (space separated) to append to the field.
| `before`            | string         |              | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`             | string         |              | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`        | array          |              | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`        | array          |              | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`          | string         |              | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`          | string         |              | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**          | ---            | ---          | ---
| `top_icon`          | string         | top-icon     | The icon/text to display on the border top field.
| `right_icon`        | string         | right-icon   | The icon/text to display on the border right field.
| `bottom_icon`       | string         | bottom-icon  | The icon/text to display on the border bottom field.
| `left_icon`         | string         | left-icon    | The icon/text to display on the border left field.
| `all_icon`          | string         | all-icon     | The icon/text to display on the border all corners field.
| `top`               | bool           | true         | Whether to show *top* of the field.
| `right`             | bool           | true         | Whether to show *right* of the field.
| `bottom`            | bool           | true         | Whether to show *bottom* of the field.
| `left`              | bool           | true         | Whether to show *left* of the field.
| `all`               | bool           | false        | Whether to show *all corners* of the field.
| `unit`              | bool           | true         | Whether to show *unit selector* of the field.
| `units`             | array          |              | The CSS measurement units, *for eg.* `px` `em` `%` `cm` `pt`
| `output`            | array\|string  |              | The CSS elements selector.
| `output_mode`       | string         | padding      | The output CSS property of an element. for eg. `relative` `padding` `margin`
| `output_important`  | bool           | false        | Whether to add **!important** rule on output CSS

<div class="pre-heading">Default Arguments</div>

| Name          | Type      | Description |
|---------------|-----------|-------------|
| `top`         | number    | A numeric value.
| `left`        | number    | A numeric value.
| `bottom`      | number    | A numeric value.
| `right`       | number    | A numeric value.
| `all`         | number    | A numeric value.
| `unit`        | string    | A defined value. *for eg.* `px` `em` `%`

----------------------------------------------------------------------------------------------------------------------------------------------

## Spinner

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Spinner w/ Default</span>
<span class="csf-tab-title">Spinner w/ Spesific</span>
<span class="csf-tab-title">Spinner w/ Output</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-spinner-1',
  'type'  => 'spinner',
  'title' => 'Spinner',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-spinner-2',
  'type'    => 'spinner',
  'title'   => 'Spinner',
  'default' => 50,
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-spinner-3',
  'type'    => 'spinner',
  'title'   => 'Spinner',
  'min'     => 0,
  'max'     => 100,
  'step'    => 10,
  'unit'    => 'px',
  'default' => 25,
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'          => 'opt-spinner-4',
  'type'        => 'spinner',
  'title'       => 'Spinner',
  'min'         => 0,
  'max'         => 1600,
  'step'        => 1,
  'unit'        => '%',
  'output'      => '.heading',
  'output_mode' => 'width',
  'default'     => 1000,
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name                | Type           | Default | Description |
|---------------------|----------------|---------|-------------|
| `id`                | string         |         | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`              | string         | spinner | The type of the field.
| `title`             | string         |         | The title of the field.
| `default`           | string         |         | The default value to return if the option does not exist in the database
| `subtitle`          | string         |         | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`              | string         |         | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`              | string         |         | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`             | string         |         | The extra CSS classes (space separated) to append to the field.
| `before`            | string         |         | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`             | string         |         | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`        | array          |         | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`        | array          |         | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`          | string         |         | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`          | string         |         | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**          | ---            | ---     | ---
| `max`               | number         | 100     | The maximum allowed value.
| `min`               | number         | 0       | The minimum allowed value.
| `step`              | number         | 1       | Amount of increment value for each step.
| `unit`              | string         | px      | The unit to display of the field, also sets output CSS property unit value.
| `output`            | array\|string  |         | The CSS elements selector.
| `output_mode`       | string         | width   | The output CSS property of an element. for eg. `width` `height` `max-width` etc.
| `output_important`  | bool           | false   | Whether to add **!important** rule on output css

----------------------------------------------------------------------------------------------------------------------------------------------

## Switcher

<div class="pre-heading">Config Examples</div>

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Switcher w/ Label</span>
<span class="csf-tab-title">Switcher w/ Dependency</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-switcher-1',
  'type'  => 'switcher',
  'title' => 'Switcher',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-switcher-2',
  'type'    => 'switcher',
  'title'   => 'Switcher',
  'label'   => 'Do you want activate it ?',
  'default' => true
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'         => 'opt-switcher-3' // field id
  'type'       => 'switcher',
  'title'      => 'Switcher',
  'default'    => true
),

// A text field with dependency conditions
array(
  'id'         => 'opt-text-1',
  'type'       => 'text',
  'title'      => 'Text',
  'dependency' => array( 'opt-switcher-3', '==', 'true' ) // check for true/false by field id
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name          | Type     | Default   | Description |
|---------------|----------|-----------|-------------|
| `id`          | string   |           | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`        | string   | switcher  | The type of the field.
| `title`       | string   |           | The title of the field.
| `default`     | string   |           | The default value to return if the option does not exist in the database
| `subtitle`    | string   |           | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`        | string   |           | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`        | string   |           | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`       | string   |           | The extra CSS classes (space separated) to append to the field.
| `before`      | string   |           | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`       | string   |           | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`  | array    |           | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`  | array    |           | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`    | string   |           | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`    | string   |           | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**    | ---      | ---       | ---
| `label`       | string   |           | The text to display with the switcher

----------------------------------------------------------------------------------------------------------------------------------------------

## Tabbed

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Tabbed w/ Default</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'            => 'opt-tabbed-1',
  'type'          => 'tabbed',
  'title'         => 'Tabbed',
  'tabs'          => array(
    array(
      'title'     => 'Tab 1',
      'icon'      => 'fa fa-heart',
      'fields'    => array(
        array(
          'id'    => 'opt-text-1',
          'type'  => 'text',
          'title' => 'Text',
        ),
      )
    ),
    array(
      'title'     => 'Tab 2',
      'icon'      => 'fa fa-gear',
      'fields'    => array(
        array(
          'id'    => 'opt-color-1',
          'type'  => 'color',
          'title' => 'Color',
        ),
      )
    ),
  )
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'            => 'opt-tabbed-2',
  'type'          => 'tabbed',
  'title'         => 'Tabbed',
  'tabs'          => array(
    array(
      'title'     => 'Tab 1',
      'icon'      => 'fa fa-heart',
      'fields'    => array(
        array(
          'id'    => 'opt-text-1',
          'type'  => 'text',
          'title' => 'Text 1',
        ),
        array(
          'id'    => 'opt-text-2',
          'type'  => 'text',
          'title' => 'Text 2',
        ),
      )
    ),
    array(
      'title'     => 'Tab 2',
      'icon'      => 'fa fa-star',
      'fields'    => array(
        array(
          'id'    => 'opt-color-1',
          'type'  => 'color',
          'title' => 'Color 1',
        ),
        array(
          'id'    => 'opt-color-2',
          'type'  => 'color',
          'title' => 'Color 2',
        ),
      )
    ),
  ),
  'default'       => array(
    'opt-text-1'  => 'This is text 1 value',
    'opt-text-2'  => 'This is text 2 value',
    'opt-color-1' => '#555',
    'opt-color-2' => '#999',
  )
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name          | Type    | Default | Description |
|---------------|---------|---------|-------------|
| `id`          | string  |         | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`        | string  | tabbed  | The type of the field.
| `title`       | string  |         | The title of the field.
| `default`     | array   |         | The default value to return if the option does not exist in the database
| `subtitle`    | string  |         | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`        | string  |         | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`        | string  |         | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`       | string  |         | The extra CSS classes (space separated) to append to the field.
| `before`      | string  |         | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`       | string  |         | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`  | array   |         | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`  | array   |         | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`    | string  |         | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`    | string  |         | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**    | ---     | ---     | ---
| `tabs`        | array   |         | An associative array containing fields for the fieldsets.

----------------------------------------------------------------------------------------------------------------------------------------------

## Text

<div class="pre-heading">Config Example</div>

```php
array(
  'id'      => 'opt-text',
  'type'    => 'text',
  'title'   => 'Text',
  'default' => 'Hello world.'
),
```

<div class="pre-heading">Usage</div>

```php
$my_options = get_option( 'my_framework' ); // prefix of framework
echo $my_options['opt-text']; // id of field
```

<div class="pre-heading">Arguments</div>

| Name           | Type    | Default | Description |
|----------------|---------|---------|-------------|
| `id`           | string  |         | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`         | string  | text    | The type of the field.
| `title`        | string  |         | The title of the field.
| `default`      | string  |         | The default value to return if the option does not exist in the database
| `subtitle`     | string  |         | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`         | string  |         | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`         | string  |         | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`        | string  |         | The extra CSS classes (space separated) to append to the field.
| `before`       | string  |         | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`        | string  |         | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`   | array   |         | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`   | array   |         | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`     | string  |         | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`     | string  |         | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**     | ---     | ---     | ---
| `placeholder`  | string  |         | The placeholder to be displayed when nothing is typed.

----------------------------------------------------------------------------------------------------------------------------------------------

## Textarea

<div class="pre-heading">Config Example</div>

```php
array(
  'id'      => 'opt-textarea',
  'type'    => 'textarea',
  'title'   => 'Textarea',
  'default' => 'Lorem ipsum dollar.'
),
```

<div class="pre-heading">Usage</div>

```php
$my_options = get_option( 'my_framework' ); // prefix of framework
echo $my_options['opt-textarea']; // id of field
```

<div class="pre-heading">Arguments</div>

| Name           | Type           | Default   | Description |
|----------------|----------------|-----------|-------------|
| `id`           | string         |           | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`         | string         | textarea  | The type of the field.
| `title`        | string         |           | The title of the field.
| `default`      | string         |           | The default value to return if the option does not exist in the database
| `subtitle`     | string         |           | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`         | string         |           | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`         | string         |           | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`        | string         |           | The extra CSS classes (space separated) to append to the field.
| `before`       | string         |           | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`        | string         |           | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`   | array          |           | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`   | array          |           | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`     | string         |           | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`     | string         |           | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**     | ---            | ---       | ---
| `placeholder`  | string         |           | The placeholder to be displayed when nothing is typed.
| `shortcoder`   | array\|string  |           | The call a shortcode trigger button by shortcode id(s).

----------------------------------------------------------------------------------------------------------------------------------------------

## Typography

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Typography w/ Default</span>
<span class="csf-tab-title">Typography w/ Output</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-typography-1',
  'type'  => 'typography',
  'title' => 'Typography',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-typography-2',
  'type'    => 'typography',
  'title'   => 'Typography',
  'default' => array(
    'color'       => '#ffbc00',
    'font-family' => 'Open Sans',
    'font-size'   => '16',
    'line-height' => '20',
    'unit'        => 'px',
    'type'        => 'google',
  ),
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'      => 'opt-typography-3',
  'type'    => 'typography',
  'title'   => 'Typography',
  'output'  => '.heading',
  'default' => array(
    'color'          => '#ffbc00',
    'font-family'    => 'Barlow',
    'font-size'      => '16',
    'line-height'    => '20',
    'letter-spacing' => '-1',
    'text-align'     => 'center',
    'text-transform' => 'uppercase',
    'subset'         => 'latin-ext',
    'type'           => 'google',
    'unit'           => 'px',
  ),
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name                 | Type           | Default    | Description |
|----------------------|----------------|------------|-------------|
| `id`                 | string         |            | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`               | string         | typography | The type of the field.
| `title`              | string         |            | The title of the field.
| `default`            | array          |            | The default value to return if the option does not exist in the database
| `subtitle`           | string         |            | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`               | string         |            | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`               | string         |            | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`              | string         |            | The extra CSS classes (space separated) to append to the field.
| `before`             | string         |            | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`              | string         |            | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`         | array          |            | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`         | array          |            | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`           | string         |            | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`           | string         |            | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**           | ---            | ---        | ---
| `font_family`        | bool           | true       | Whether to show *font_family* of the field. (specifies the font)
| `font_weight`        | bool           | true       | Whether to show *font_weight* of the field. (sets the size of a font)
| `font_style`         | bool           | true       | Whether to show *font_style* of the field. (specifies the font style)
| `font_size`          | bool           | true       | Whether to show *font_size* of the field. (sets the size of a font)
| `line_height`        | bool           | true       | Whether to show *line_height* of the field. (specifies the height of a line)
| `letter_spacing`     | bool           | true       | Whether to show *letter_spacing* of the field. (increases or decreases the space between characters in a text)
| `text_align`         | bool           | true       | Whether to show *text_align* of the field. (specifies the horizontal alignment of text in an element)
| `text_transform`     | bool           | true       | Whether to show *text_transform* of the field. (controls the capitalization of text)
| `color`              | bool           | true       | Whether to show *color* of the field. (specifies the color of text)
| `subset`             | bool           | true       | Whether to show *subset* of the field. (specifies the languages of font)
| `chosen`             | bool           | true       | Whether to enable [ChosenJS](https://harvesthq.github.io/chosen/) style select.
| `preview`            | bool           | true       | Whether to show *preview font area* of the field.
| `backup_font_family` | bool           | false      | Whether to show *backup_font_family* of the field. (specifies the generic font family backup)
| `font_variant`       | bool           | false      | Whether to show *font_variant* of the field. (specifies whether or not a text should be displayed in a small-caps font)
| `word_spacing`       | bool           | false      | Whether to show *word_spacing* of the field. (increases or decreases the white space between words.)
| `text_decoration`    | bool           | false      | Whether to show *text_decoration* of the field. (specifies the decoration added to text)
| `custom_style`       | bool           | false      | Whether to show *custom_style* of the field.
| `extra_styles`       | bool           | false      | Whether to show *extra_styles* of the field. (sets allows multiple choose the font styles)
| `exclude`            | string         |            | Define a comma-separated list of font family group to be excluded from the list. *for eg.* `google` `custom,safe`
| `unit`               | string         | px         | The unit to display on the border inputs, also sets output CSS property unit value.
| `output`             | array\|string  |            | The CSS elements selector.
| `output_important`   | bool           | false      | Whether to add **!important** rule on output CSS

<div class="pre-heading">Default Arguments</div>

| Name                 | Type     | Description |
|----------------------|----------|-------------|
| `color`              | string   | A validated color value. *for eg.* `#1e73be`, `rgba(255,0,0,0.25)`
| `font-family`        | string   | A font family value. *for eg.* `Open Sans` `Roboto` `Arial`
| `backup-font-family` | string   | A font family value. *for eg.* `Arial, Helvetica, sans-serif`
| `font-weight`        | string   | A defined value. *for eg.* `100` `200` `300` `normal` `500` `600` `700` `800` `900`
| `font-style`         | string   | A defined value. *for eg.* `normal` `italic`
| `font-size`          | number   | A numeric value.
| `line-height`        | number   | A numeric value.
| `letter-spacing`     | number   | A numeric value.
| `word-spacing`       | number   | A numeric value.
| `text-align`         | string   | A defined value. *for eg.* `left` `center` `right` `justify`
| `text-transform`     | string   | A defined value. *for eg.* `none` `capitalize` `uppercase` `lowercase`
| `font-variant`       | string   | A defined value. *for eg.* `normal` `small-caps` `all-small-caps`
| `text-decoration`    | string   | A defined value. *for eg.* `none` `underline` `underline dotted` `underline dashed`
| `custom-style`       | string   | A defined value. *for eg.* `text-shadow: 1px 1px 1px red`
| `extra-styles`       | array    | A defined value. *for eg.* `100` `100italic` `200` `200italic` `...` `900` `900italic`
| `type`               | string   | A defined value. *for eg.* `google` `safe` `custom`
| `subset`             | string   | A defined value. *for eg.* `latin` `latin-ext`
| `unit`               | string   | A defined value. *for eg.* `px` `em` `rem` `%`

----------------------------------------------------------------------------------------------------------------------------------------------

## Upload

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">Upload only Images</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
 array(
  'id'    => 'opt-upload-1',
  'type'  => 'upload',
  'title' => 'Upload',
),
```
</div>
<div class="csf-tab-content">

```php
 array(
  'id'           => 'opt-upload-2',
  'type'         => 'upload',
  'title'        => 'Upload',
  'library'      => 'image',
  'placeholder'  => 'http://',
  'button_title' => 'Add Image',
  'remove_title' => 'Remove Image',
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name              | Type           | Default    | Description |
|-------------------|----------------|------------|-------------|
| `id`              | string         |            | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`            | string         | upload     | The type of the field.
| `title`           | string         |            | The title of the field.
| `default`         | string         |            | The default value to return if the option does not exist in the database
| `subtitle`        | string         |            | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`            | string         |            | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`            | string         |            | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`           | string         |            | The extra CSS classes (space separated) to append to the field.
| `before`          | string         |            | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`           | string         |            | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`      | array          |            | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`      | array          |            | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`        | string         |            | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`        | string         |            | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**        | ---            | ---        | ---
| `library`         | array\|string  | all        | Tell the modal to show specific formats. for eg. `image` or `video` or both etc.
| `placeholder`     | string         |            | The placeholder to be displayed when nothing is selected.
| `button_title`    | string         | Upload     | The text to display on the upload button.
| `remove_title`    | string         | Remove     | The text to display on the remove button.

---

## WP Editor

<div class="pre-heading">Config Examples</div>
<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Simple</span>
<span class="csf-tab-title">WP Editor w/ Custom Settings</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">

```php
array(
  'id'    => 'opt-wp-editor-1',
  'type'  => 'wp_editor',
  'title' => 'WP Editor',
),
```
</div>
<div class="csf-tab-content">

```php
array(
  'id'       => 'opt-wp-editor-2',
  'type'     => 'wp_editor',
  'title'    => 'WP Editor',
  'settings' => array(
    'textarea_rows' => 5,
    'tinymce'       => false,
    'media_buttons' => false,
  )
),
```
</div>
</div>
<div class="clear"></div>
</div>

<div class="pre-heading">Arguments</div>

| Name          | Type    | Default    | Description |
|---------------|---------|------------|-------------|
| `id`          | string  |            | A unique **slug-like ID**. This **ID** will be used to get the value.
| `type`        | string  | wp_editor  | The type of the field.
| `title`       | string  |            | The title of the field.
| `default`     | string  |            | The default value to return if the option does not exist in the database
| `subtitle`    | string  |            | The subtitle to display below the title. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `desc`        | string  |            | The description to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `help`        | string  |            | The text to display on right-corner (as hover/popup) the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `class`       | string  |            | The extra CSS classes (space separated) to append to the field.
| `before`      | string  |            | The content to display before the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `after`       | string  |            | The content to display after the field. <a href="#/faq?id=how-to-use-common-arguments" class="csf-more-link">?</a>
| `dependency`  | array   |            | The show/hide to fields based on rules. <a href="#/faq?id=how-to-use-dependencies" class="csf-more-link">?</a>
| `attributes`  | array   |            | The extra HTML attributes to append to the field. <a href="#/faq?id=how-to-use-attributes" class="csf-more-link">?</a>
| `sanitize`    | string  |            | The callback function for sanitizing value. <a href="#/faq?id=how-to-use-sanitize" class="csf-more-link">?</a>
| `validate`    | string  |            | The callback function for validating value. <a href="#/faq?id=how-to-use-validate" class="csf-more-link">?</a>
| **Extras**    | ---     | ---        | ---
| `settings`    | array   |            | An associative array containing arguments for the setting.

<div class="pre-heading">Settings Arguments</div>

| Name             | Type         | Default    | Description |
|------------------|--------------|------------|-------------|
| `textarea_rows`  | number       | 10         | The number of rows to display for the textarea.
| `tinymce`        | bool         | true       | Load TinyMCE, can be used to pass settings directly to TinyMCE using an array.
| `media_buttons`  | bool         | true       | Whether to display media insert/upload buttons.

Get more informations for [wp_editor arguments](https://codex.wordpress.org/Function_Reference/wp_editor#Arguments)

---

## Others

<div class="csf-tabs">
<div class="csf-tab-buttons">
<span class="csf-tab-title csf-tab-active">Heading</span>
<span class="csf-tab-title">Subheading</span>
<span class="csf-tab-title">Submessage</span>
<span class="csf-tab-title">Notice</span>
<span class="csf-tab-title">Content</span>
</div>
<div class="csf-tab-contents">
<div class="csf-tab-content csf-tab-active">
<div class="pre-heading">Config Examples</div>

```php
// A Heading
array(
  'type'    => 'heading',
  'content' => 'This is a heading field',
),
```

<div class="pre-heading">Arguments</div>

| Name       | Type    | Default  | Description |
|------------|---------|----------|-------------|
| `type`     | string  | content  | The type of the field.
| `content`  | string  |          | The content of the field.

</div>
<div class="csf-tab-content">
<div class="pre-heading">Config Examples</div>

```php
// A Subheading
array(
  'type'    => 'subheading',
  'content' => 'This is subheading field',
),
```

<div class="pre-heading">Arguments</div>

| Name       | Type    | Default     | Description |
|------------|---------|-------------|-------------|
| `type`     | string  | subheading  | The type of the field.
| `content`  | string  |             | The content of the field.

</div>
<div class="csf-tab-content">
<div class="pre-heading">Config Examples</div>

```php
// A Submessage
array(
  'type'    => 'submessage',
  'style'   => 'success',
  'content' => 'This is a submessage field. And using style "success"',
),
```

<div class="pre-heading">Arguments</div>

| Name       | Type    | Default     | Description |
|------------|---------|-------------|-------------|
| `type`     | string  | submessage  | The type of the field.
| `style`    | string  | normal      | The style of the field. *for eg.* `normal` `success` `info` `warning` `danger`
| `content`  | string  |             | The content of the field.

</div>
<div class="csf-tab-content">
<div class="pre-heading">Config Examples</div>

```php
// A Notice
array(
  'type'    => 'notice',
  'style'   => 'success',
  'content' => 'This is a notice field. And using style "success"',
),
```

<div class="pre-heading">Arguments</div>

| Name       | Type    | Default | Description |
|------------|---------|---------|-------------|
| `type`     | string  | notice  | The type of the field.
| `style`    | string  | normal  | The style of the field. *for eg.* `normal` `success` `info` `warning` `danger`
| `content`  | string  |         | The content of the field.

</div>
<div class="csf-tab-content">
<div class="pre-heading">Config Examples</div>

```php
// A Content Field Example
array(
  'type'    => 'content',
  'content' => 'This is a content field. You can write some html here.',
),
```
<div class="pre-heading">Arguments</div>

| Name       | Type    | Default  | Description |
|------------|---------|----------|-------------|
| `type`     | string  | content  | The type of the field.
| `content`  | string  |          | The content of the field.

</div>
</div>
<div class="clear"></div>
</div>
