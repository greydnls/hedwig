Hedwig
========

###Abstraction Layer around Email Lists

Hedwig is meant to abstract away Mailing List providers. 

**Target Providers**
  * MailChimp
  * ExactTarget
  * ActiveCampaign
  

**Main Objects in Use**
  * List
  * ListMember
  
**API**

```php 
$newsletter = Hedwig::create('mailchimp'); 

$user = new Listmember();

$campaign = $newsletter->findCampaign('some_campaign');

$campaign->subscribe($user);

$campaign->unsubscribe($user);

```
