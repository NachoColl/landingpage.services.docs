---
title: Help Pages

language_tabs:
 - notes: Notes


search: false
---

# Introduction

```notes
Use mustache.website to send your Email Marketing
and host your Landing Pages! 
```

[mustache.website](https://mustache.website) is a service you can use to manage your **Contact List**, send **Email Marketing** and host your **Landing Pages**. By using state-of-the-art [Amazon Web Services](https://aws.amazon.com/) features, [mustache.website](https://mustache.website) delivers a professional tool at the minimum cost. 

You get the same, for less.

## Service Support

```notes
Do not hesitate to create a new issue
if you need help.
```

If you found an issue, please click [here](https://github.com/NachoColl/mustache.website.docs/issues) to open a new ticket or contact [me](https://www.linkedin.com/in/ignaciocoll/) on LinkedIn.


# Contacts List

To manage your contact list you can manually add contacts, import your Contacts from a [CSV file](https://en.wikipedia.org/wiki/Comma-separated_values) or use the available API to manage your contacts programmatically.


## Adding Contacts

```notes
Please note that the Email attribute is a key 
value that cannot be changed after creation. 

If you need to change a contact email, you must 
delete it and create a new contact.
```

To add a new contact, just select **My Contacts > Contact List** menu option and then click on the **New Contact** button. Enter the contact attributes and click on the Save button.

<img src="images/new-contact.jpg" class="img-photo" />




## Import Contacts

```notes
It's recommended that you initially 
try to import some small files with 
a few records to check the results.
```

Before you start, please check that your [CSV file](https://en.wikipedia.org/wiki/Comma-separated_values) follows the next rules:

- The first row contains the column names.
- There is an Email attribute column.
- Values are Numbers, Texts or Dates.
- Date columns use one of the allowed formats:
    * DD/MM/YYYY, e.g. 24/03/2017
    * MM/DD/YYYY, e.g. 01/25/2015
    * [Unix time](https://en.wikipedia.org/wiki/Unix_time) format (milliseconds), e.g. 1492364709813 representing Sun Apr 16 2017 19:45:09 GMT+0200.

<br/>

To start the import process click on **My Contacts > Import** menu option and select your CSV file. 

<img src="images/import-contact-select-file.jpg" class="img-photo" />

```notes
Double check your CSV file column mapping!
```

Take a look at the columns mapping that it's proposed and select the appropiate option for each column.

<img src="images/import-contact-mapping.jpg" class="img-photo" />

```notes
When you click the Start Import button, the 
CSV file is sent to the system and 
each row is then processed. 
```

Once you've finished mapping your CSV file columns, click on the **Start Import** button to start the import process.

```notes
You will get the import results on your 
account email, including the total
processed contacts and the total 
imported contacts number.

If there are errors while processing 
the file, you will also get some 
error details.
```

<img src="images/import-contact-result.jpg" class="img-photo" />



## Target Groups

```notes
If no new Target Groups are created, you're 
just going to be able to send a Campaign 
to all your contacts.
```

When you create a new Email Marketing campaign, you select the [Target Group](https://en.wikipedia.org/wiki/Target_audience) to which you want to send the message. That means that if you want to send your campaign to an specific group of contacts, you have to create a new Target Group that defines that group (e.g. Canada Users).

```notes
A Target Group is a database filter 
definition.
```
<br/>

To create a target group, go to **My Contacts > Contact List** and click on the **Target Groups** button.


<img src="images/target-group-create.jpg" class="img-photo" />

```notes
Before saving a new Target Group, click on 
the Search button to test the filter.
```

Add the attributes values that define your target group, enter a Target Group name and click on the **Save as NEW target group** button.


# Email Campaigns

To create a new Email Campaign go to **Email Marketing > Campaigns** and click on **New Campaign** button. Enter a campaign name, select the Target Group you want to send the email message and click on the **Save** button.

<img src="images/campaign-select-target-group.jpg" class="img-photo" />


## Message Content

After you've set the campaign name and Target Group, click on the campaign **email content** button to setup the campaign email message. 

<img src="images/campaign-create.jpg" class="img-photo" />

```notes
You can change the base template HTML code
when required to get the email message 
format you need.
```

The first time you click on the **email content** button you will get the option to select the base template you want to start building your campaign email. Check for the available templates and select the option that best fits your needs.

<img src="images/campaign-select-base-template.jpg" class="img-photo" />

If you take a look at the next image, the content is defined by filling the text areas on the right, and not directly on the HTML preview.

```notes
mustache.website templates use the 
{{mustache}} technique so you can 
build your content by just filling 
a few textboxes.
```

<img src="images/campaign-mail-content.jpg" class="img-photo" />

If the selected template needs some modifications to fit your needs, you can change the HTML code. Click on the **Change HTML Code** button, and an HTML editor will be displayed. Just take care that if you want to add a new mustache, you must use the correct format.

<img src="images/campaign-mail-content-change-html-code.jpg" class="img-photo" />


## Campaign Execution

Once your campaign is ready go to **Email Marketing > Campaigns** list and click on the **run the campaign** to start sending the email messages to your contacts. 

```notes
You can pause a campaign by just
selecting the Stop campaign option.
```

<img src="images/campaign-options.jpg" class="img-photo" />

While running, you will get updates indicating the number of messages sent, delivered and the related bounces and complaints.


# Landing Pages

```notes
HTML pages are saved on AWS S3 bucket 
as static HTML pages. 

Please note that you can use your own domain(s)
to access your pages.
```

[mustache.website](https://mustache.website) landing pages are created by selecting an HTML template with some {{[mustaches](http://mustache.github.io/)}} that define the areas you can change. To create a new web page then you just need to select a template and fill the {{mustaches}}. 

There is no need to go through a new HTML design process every time!

## WEB Templates

> A WEB template example.

```notes

<!DOCTYPE html>
<html>

<head>
    <title>{{meta-page_title-the_page_title}}</title>
</head> 

<html>
<body>
    
    <h1>{{text-header_text-big_text}}</h1>
    
</body>
</html>
```

Before you can go for your landing pages you need to create at least one template. To start, select **Landing Pages > WEB Templates** menu option and click on the **New Template** button. 

<img src="images/landing-page-new.jpg" class="img-photo"/>

Check the available base templates you can start from, and click on the **Select** button for the selected template.

```notes
You can also start to code your template 
from scratch if required!
```

<img src="images/landing-page-select-base-template.jpg" class="img-photo"/>


```notes

Just fill the 'mustaches', click save, and your 
landing page will be online!

```

Once selected, you will get an HTML editor so you can change the HTML. Just remember to use {{mustaches}} to the define the areas that will be required to modify when building the page later.

<img src="images/landing-page-html-editor.jpg" class="img-photo"/>
 
### Adding mustaches

To make things easy when building your landing pages, we added different types of mustaches that are coded as follows: 

`{{<meta|text|icon|image|link|html>-<name>-<description>}}`

<img src="images/template-mustache.png"  class="img-photo" />

```notes
To insert a mustache in your HTML code, 
you must use the correct format.

We recommend that you use the Insert Mustache
button.

```

* **Meta** mustaches are used to set meta properties content.<br/> `{{{meta-page_title-the_page_title}}}`

* **Only Text** to include non-formatted text (format is already set on the template!).<br/> `{{{text-header_content-the_headear_title}}}`

* **Icon** so you can easely include a [Simple Icon](http://simplelineicons.com/) on your page. <br/> `{{{icon-feature-app_feature_icon}}}`

* **Image** to upload your images and use them when required. <br/> `{{{image-app_snapshot-product_snapshot}}}`

* **Link** to add references between your landing pages. <br/> `{{{link-download_link-the_app_download_link}}}`

* and **HTML** to add any extra HTML code your page may require. <br/> `{{{html-google-google_analytics_code}}}`

<br/>
By using those types, you get some extra help on page creation. For example, if you set an Icon mustache, you will get a button to select the icon from a list.

<img src="images/landingpage.icon-mustache.png"  class="img-photo" />


## Landing Page

```notes
Using WEB Templates you don't
have to do any design decision 
when building your pages.

```

To build and get online your landing page, click on **Landing Pages > My Pages** menu option and then click on the **New Landing Page** button. 

<img src="images/landing-page-build.jpg" class="img-photo"/>

You will get a form to set a page name, a description and select the template you want to use. 

The key point is that when the template gets selected, all the related {{mustaches}} will get listed so you only have to fill the related boxes and save your work to get your page online.

```notes
When saved, the page will get visible 
on the Internet.
```

<aside class="warning">
IMPORTANT NOTE: once saved, the page name cannot be changed.
</aside>

```notes
If you change the template, all the 
previous values may be deleted.
```

<img src="images/landingpage.page-update-mustaches.png"  class="img-photo" />

### Default URL

When your page gets saved, it's hosted on AWS S3 instantly. To check how it looks, just go to your page default address by clicking on the top page link.

<img src="images/landingpage-page-update-link.png"  class="img-photo" />

That link will look like `https://s3-us-west-2.amazonaws.com/files.landingpage.services/us-west-2:ca67230b-4f84-43bb-96d7-7fcbfdf1a034/My-first-page.html`, but of course you can use your own domain(s) if it's required.


### Use your domain(s)

```notes
A page can have multiple domains pointing to it!
```

To use your own domain create a new page as described above and click on the **Options*+ button.

<aside class="notice">
The Options button will only get displayed after saving your page.
</aside>

<img src="images/landingpage-page-update-options.png"  class="img-photo" />

A popup will be displayed. Enter your domain (e.g. www.mydomain.com) and click on the **Add** button. Also remember to check the Default Page option if you want the current to get displayed as the default domain page.

<img src="images/landingpage.page-update-add-domain.png"  class="img-photo" />

Please note that you also need to add a CNAME entry on your domain's DNS server.

`www.mydomain.com   CNAME   ec2-52-38-184-2.us-west-2.compute.amazonaws.com`

<br/><br/>

<span style="font-size:10px">This is THE END ;)</span>







