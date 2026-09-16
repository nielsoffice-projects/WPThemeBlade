# WPThemeBlade-
WPThemeBlade 


```
// Generate Theme
WP underscore 

// Install loader
composer init

// Install Dependency 
composer require roots/acorn


<?php

require_once __DIR__ . '/vendor/autoload.php';

add_action('after_setup_theme', function () {
    if (function_exists('Roots\bootloader')) {
        \Roots\bootloader()->boot();
    }
});


my-theme/
├── resources/
│   └── views/
│       ├── home.blade.php
│       ├── header.blade.php
│       └── footer.blade.php
├── vendor/
├── functions.php
└── style.css


// Execution Index.php  
<?php

echo view('home')->render();


// USAGE: 

<h1>{{ get_the_title() }}</h1>

<div>
    {!! get_the_content() !!}
</div>

{{ $variable }}


```

```

my-theme/
├── app/
│   ├── Controllers/
│   └── ...
├── resources/
│   ├── views/
│   │   ├── layouts/
│   │   │   └── app.blade.php
│   │   ├── components/
│   │   ├── partials/
│   │   ├── home.blade.php
│   │   ├── single.blade.php
│   │   └── page.blade.php
│   ├── css/
│   └── js/
├── public/
├── vendor/
├── composer.json
├── functions.php
├── index.php
└── style.css



