# WPThemeBlade Development
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
│   ├── setup.php
│   ├── filters.php
│   └── helpers.php
│
├── config/
│   └── app.php
│
├── resources/
│   ├── views/
│   │   ├── layouts/
│   │   │   └── app.blade.php
│   │   │
│   │   ├── partials/
│   │   │   ├── header.blade.php
│   │   │   ├── footer.blade.php
│   │   │   ├── navigation.blade.php
│   │   │   └── sidebar.blade.php
│   │   │
│   │   ├── components/
│   │   │   ├── button.blade.php
│   │   │   ├── card.blade.php
│   │   │   └── post-card.blade.php
│   │   │
│   │   ├── pages/
│   │   │   ├── home.blade.php
│   │   │   ├── about.blade.php
│   │   │   └── contact.blade.php
│   │   │
│   │   ├── single.blade.php
│   │   ├── page.blade.php
│   │   ├── archive.blade.php
│   │   ├── search.blade.php
│   │   └── 404.blade.php
│   │
│   ├── css/
│   │   └── app.css
│   │
│   └── js/
│       └── app.js
│
├── public/
│   ├── images/
│   └── fonts/
│
├── functions.php
├── index.php
├── style.css
├── screenshot.png
├── composer.json
├── package.json
└── theme.json



```

<BR> READ MORE: https://roots.io/acorn/docs/?utm_source=chatgpt.com
<BR> Website: https://roots.io/
