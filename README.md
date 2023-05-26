# Complete Modern Design for Contact Form 7
Modern look for the [Contact Form 7](https://wordpress.org/plugins/contact-form-7/) WordPress plugin – a complete CSS style sheet
<br>
<br>
![CF7 Modern Design - Overview](https://github.com/lukaspodmelle/contact-form-7-modern-design/assets/132982113/da6a44df-f658-400e-b343-9942a90d28e1)

<h3>Description</h3>

This is a CSS style sheet to replace the default styles of the **Contact Form 7** WordPress plugin. Covers all available input types, validation, responses and also features **custom radio buttons and checkboxes.**

<ul>
  <li>All text fields</li>
  <li>Dropdown menu</li>
  <li>File upload</li>
  <li>Date picker</li>
  <li>Custom radio buttons</li>
  <li>Custom checkboxes</li>
  <li>Validation styles</li>
  <li>Response messages</li>
</ul>

<h3>Easy customization</h3>

The CSS file includes a <code>:root</code> section for **easy customization based on your theme styles.** Simply change the HEX codes or font.

```
:root {
    --cf7-font: inherit;
    --cf7-font-size: 16px;
    --cf7-font-weight: 300;
    --cf7-labels: #5a6e81;
    --cf7-input-text: #8CA3B9;
    --cf7-accent: #2d8cff;
    --cf7-accent-hover: #247de9;
    --cf7-accent-outline: #b9d9ff;
    --cf7-accent-text: #ffffff;
    --cf7-warning: #fb584e;
    --cf7-warning-bg: #FFEDEC;
    --cf7-success: #00B474;
    --cf7-success-bg: #E6FFF0;
}
```

<h3>Installation</h3>

**Option 1.** Paste the contents of "style.css" into your WordPress Customizer -> Custom CSS
<br>(or any other global Custom CSS field available in your theme)
<br>
<br>
**Option 2.** Create a separate "cf7-styles.css" file in your (child) theme folder and enqueue it in functions.php

```
<?php
wp_enqueue_style('cf7-styles', get_template_directory_uri() . "/cf7-styles.css", array(), '1.0');
?>
```

<h3>Note</h3>

The font used in the preview is a Google Font called [Outfit](https://fonts.google.com/specimen/Outfit). In case you want to keep it, you can append to the file:

```
@import url('https://fonts.googleapis.com/css2?family=Outfit:wght@300;400;500;600;700;800&display=swap'); 
```

And don't forget to change it in the <code>:root</code> as well:
```
:root {
    --cf7-font: 'Outfit';
```
