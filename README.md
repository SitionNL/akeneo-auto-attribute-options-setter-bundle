# AutoAttributeOptionsSetterBundle

This bundle ensure that attribute options are created automatically when importing products for simple select and multi select attribute.

## Installation

- Execute the following command to add the dependency to your `composer.json`

`composer require niji/auto-attribute-options-setter-bundle`

- In your app/AppKernel.php add a line to enable the bundle:
   
```php
public function registerProjectBundles() {
  return [
      // your app bundles should be registered here,
      .../...
      new Niji\AutoAttributeOptionsSetterBundle\AutoAttributeOptionsSetterBundle(),
      .../...
  ];
}
```

## Clean cache 
- first go to your akeneo install folder
`php bin/console cache:clear --no-warmup --env=prod`

- Clean your browser cache, navigat to system -> system information, under registered bundles now you should see: 
Niji\AutoAttributeOptionsSetterBundle\AutoAttributeOptionsSetterBundle

## Credits

This bundle is brought to you by Niji - http://www.niji.fr.
