##Hi!

```
require('profile');
require('tech');

$me = new Profile();
$tech = new Technologies();

$me->setName('Jonathas Montenegro');
$me->setJob('Web Developer');
$me->setWorkingOn([
  $tech->find('Laravel'),
  $tech->find('CakePHP'),
  $tech->find('Javascript'),  
  $tech->find('Docker'),
  $tech->find('SAP ABAP'),
  $tech->find('SAP Funcional Support'),
  $tech->find('SAP Odata Webservices')
]);

$me->defineFuture(($me, $tech) => {
   while($tech->findNewTechnologies()){
      $me->learn();
   }
});
```
