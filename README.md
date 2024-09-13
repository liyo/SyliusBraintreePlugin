# [![](https://bitbag.io/wp-content/uploads/2020/10/braintree.png)](https://bitbag.io/?utm_source=github&utm_medium=referral&utm_campaign=plugins_braintree) 

# BitBag SyliusBraintreePlugin
----

[![](https://img.shields.io/packagist/l/bitbag/braintree-plugin.svg) ](https://packagist.org/packages/bitbag/braintree-plugin "License") [ ![](https://img.shields.io/packagist/v/bitbag/braintree-plugin.svg) ](https://packagist.org/packages/bitbag/braintree-plugin "Version") [ ![](https://img.shields.io/github/actions/workflow/status/BitBagCommerce/SyliusBraintreePlugin/build.yml?branch=master) ](https://github.com/BitBagCommerce/SyliusBraintreePlugin/actions "Build status") [ ![](https://img.shields.io/scrutinizer/g/BitBagCommerce/SyliusBraintreePlugin.svg) ](https://scrutinizer-ci.com/g/BitBagCommerce/SyliusBraintreePlugin "Scrutinizer") [![](https://poser.pugx.org/bitbag/braintree-plugin/downloads)](https://packagist.org/packages/bitbag/braintree-plugin "Total Downloads") [![Slack](https://img.shields.io/badge/community%20chat-slack-FF1493.svg)](http://sylius-devs.slack.com) [![Support](https://img.shields.io/badge/support-contact%20author-blue])](https://bitbag.io/contact-us/?utm_source=github&utm_medium=referral&utm_campaign=plugins_braintree)

We want to impact many unique eCommerce projects and build our brand recognition worldwide, so we are heavily involved in creating open-source solutions, especially for Sylius. We have already created over **35 extensions, which have been downloaded almost 2 million times.**

You can find more information about our eCommerce services and technologies on our website: https://bitbag.io/. We have also created a unique service dedicated to creating plugins: https://bitbag.io/services/sylius-plugin-development. 

Do you like our work? Would you like to join us? Check out the **“Career” tab:** https://bitbag.io/pl/kariera. 

# About Us 
---

BitBag is a software house that implements tailor-made eCommerce platforms with the entire infrastructure—from creating eCommerce platforms to implementing PIM and CMS systems to developing custom eCommerce applications, specialist B2B solutions, and migrations from other platforms.

We actively participate in Sylius's development. We have already completed **over 150 projects**, cooperating with clients worldwide, including smaller enterprises and large international companies. We have completed projects for such important brands as **Mytheresa, Foodspring, Planeta Huerto (Carrefour Group), Albeco, Mollie, and ArtNight.**

We have a 70-person team of experts: business analysts and consultants, eCommerce developers, project managers, and QA testers.

**Our services:**
* B2B and B2C eCommerce platform implementations
* Multi-vendor marketplace platform implementations
* eCommerce migrations
* Sylius plugin development
* Sylius consulting
* Project maintenance and long-term support
* PIM and CMS implementations

**Some numbers from BitBag regarding Sylius:**
* 70 experts on board 
* +150 projects delivered on top of Sylius
* 30 countries of BitBag’s customers
* 7 years in the Sylius ecosystem
* +35 plugins created for Sylius

---
[![](https://bitbag.io/wp-content/uploads/2024/09/badges-sylius.png)](https://bitbag.io/contact-us/?utm_source=github&utm_medium=referral&utm_campaign=plugins_elasticsearch) 

---


## Table of Content
---
* [Overview](#overview)
* [Installation](#installation)
  * [Customization](#customization)
  * [Testing](#testing)
* [Functionalities](#functionalities)
* [Demo](#demo)
* [Additional resources for developers](#additional-resources-for-developers)
* [License](#license)
* [Contact](#contact)
* [Community](#community)



# Overview
---
The Braintree Plugin seamlessly integrates the Braintree payment gateway into your Sylius eCommerce platform, enabling a straightforward and secure shopping experience for your customers. As an open-source addition to the Sylius ecosystem, this plugin brings together the comprehensive features of both Sylius and Braintree, facilitating not only payment processing but also order refunds.




# Installation
---

```bash
$ composer require bitbag/braintree-plugin 
```
    
Add plugin dependencies to your config/bundles.php file:

```php
return [
   BitBag\SyliusBraintreePlugin\BitBagSyliusBraintreePlugin::class => ['all' => true]
];
```

Import configuration:

```yaml
imports:
    ...
    
    - { resource: "@BitBagSyliusBraintreePlugin/Resources/config/config.yml" }
```

## Customization
----
### Available services you can [decorate](https://symfony.com/doc/current/service_container/service_decoration.html) and forms you can [extend](http://symfony.com/doc/current/form/create_form_type_extension.html)

Run the below command to see what Symfony services are shared with this plugin:
 
```bash
$ bin/console debug:container bitbag_sylius_braintree_plugin
```

## Testing
----
```bash
$ composer install
$ cd tests/Application
$ yarn install
$ yarn build
$ bin/console assets:install public -e test
$ bin/console doctrine:database:create -e test
$ bin/console doctrine:schema:create -e test
$ bin/console server:run 127.0.0.1:8080 -e test
$ open http://localhost:8080
$ vendor/bin/behat
$ vendor/bin/phpspec run
```
---

**If you need some help with Sylius development, don't be hesitated to contact us directly. You can fill the form on [this site](https://bitbag.io/contact-us/?utm_source=github&utm_medium=referral&utm_campaign=plugins_braintree) or send us an e-mail at hello@bitbag.io!**

---

# Functionalities
---

All main functionalities of the plugin are described [here.](https://github.com/BitBagCommerce/SyliusBraintreePlugin/blob/master/doc/functionalities.md)

# Demo 
---

We created a demo app with some useful use-cases of plugins! Visit http://demo.sylius.com/ to take a look at it.

**If you need an overview of Sylius' capabilities, schedule a consultation with our expert.**

[![](https://bitbag.io/wp-content/uploads/2020/10/button_free_consulatation-1.png)](https://bitbag.io/contact-us/?utm_source=github&utm_medium=referral&utm_campaign=plugins_braintree)

# Additional resources for developers
---
To learn more about our contribution workflow and more, we encourage you to use the following resources:
* [Sylius Documentation](https://docs.sylius.com/en/latest/)
* [Sylius Contribution Guide](https://docs.sylius.com/en/latest/contributing/)
* [Sylius Online Course](https://sylius.com/online-course/)
* [Sylius Plugins Blogs](https://bitbag.io/blog/category/plugins) 

# License
---

This plugin's source code is completely free and released under the terms of the MIT license.

[//]: # (These are reference links used in the body of this note and get stripped out when the markdown processor does its job. There is no need to format nicely because it shouldn't be seen.)

# Contact
---
This open-source plugin was developed to help the Sylius community. If you have any additional questions, would like help with installing or configuring the plugin, or need any assistance with your Sylius project - let us know! **Contact us** or send us an **e-mail to hello@bitbag.io** with your question(s).

[![](https://bitbag.io/wp-content/uploads/2020/10/button-contact.png)](https://bitbag.io/contact-us/?utm_source=github&utm_medium=referral&utm_campaign=plugins_braintree)


# Community
---- 

For online communication, we invite you to chat with us & other users on **[Sylius Slack](https://sylius-devs.slack.com/).**

[![](https://bitbag.io/wp-content/uploads/2024/09/badges-partners.png)](https://bitbag.io/contact-us/?utm_source=github&utm_medium=referral&utm_campaign=plugins_braintree)
