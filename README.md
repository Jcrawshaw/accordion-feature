# accordion-feature

This is an accordion style feature that uses html, css, and javascript. This can be used for any drop down information such as a "frequently asked question area"

[See a demo in codepen](http://codepen.io/Jcrawshaw/pen/XKdzRe "Codepen Accordion Feature")

If using this code on a Wordpress Theme, enqueue the script in the `functions.php` file with the following function:
```
//* Load scripts for accordion menu
function custom_scripts() {

wp_register_script( 'custom-script', get_stylesheet_directory_uri() . '/js/accordion.js', array() , false, true );

wp_enqueue_script( 'custom-script' );
}

add_action( 'wp_enqueue_scripts', 'custom_scripts', 99 );
```

