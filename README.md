# Extending Admin UI

This bundle helps to extend admin ui

Requirements
------------

* Ibexa 4.6+

## Install instructions

1. Add the project repository:
    
    In the main `composer.json`, add:
    ```
    "repositories": [
        // ...
        {
            "type": "vcs",
            "url": "https://github.com/rhidja/ezskeleton-bundle"
        }
    ],
    ```

2. Install the bundle via Composer (initial installation):

    ```
    $ composer require rhidja/ezskeleton-bundle
    ```
    2.1 Update the bundle via Composer if needed
    ```
    $ composer update rhidja/ezskeleton-bundle
    ```

3. Activate the bundle in your `app/AppKernel.php`:

    ```php
    $bundles = [
        ...
        new Kabylia\EzSkeletonBundle\KabyliaEzSkeletonBundle(),
        ...
    ];
    ```

4. Update app/config/routing.yml

    ```
    ibexa_udw_tab_tutorial:
        resource: "@KabyliaEzSkeletonBundle/Resources/config/routing.yml"
        prefix:   /
   ```
