---
title: CKLS Technical Prerequisites
keywords: pre-requisites, prerequisites, requirements
last_updated: 9 November, 2017
sidebar: home_sidebar
permalink: CKLS-prerequisites.html
folder: prerequisites
---


## Workstation requirements

CrossKnowledge LMS is a web-based application needing the following environment to run properly:

<table>
    <tbody>
        <tr>
            <td>Sound card</td>
            <td>Activated (headphones are required for most content)</td>
        </tr>
        <tr>
            <td>RAM</td>
            <td>2 GB (4GB prefered, depending on the OS)</td>
        </tr>
        <tr>
            <td>Screen resolution</td>
            <td>1024*768</td>
        </tr>
        <tr>
            <td>Windows operating system</td>
            <td>Windows Vista, 7, 8, 10 (Desktop mode only, Tablet mode is not supported for now)</td>
        </tr>
        <tr>
            <td>Apple operating system</td>
            <td>Mac OSX (10.4)</td>
        </tr>
        <tr>
            <td>Internet Explorer</td>
            <td>8, 9, 10, 11, latest version</td>
        </tr>
        <tr>
            <td>Microsoft Edge</td>
            <td>latest version</td>
        </tr>
        <tr>
            <td>Firefox</td>
            <td>latest version</td>
        </tr>
        <tr>
            <td>Chrome</td>
            <td>latest version</td>
        </tr>
        <tr>
            <td>Safari</td>
            <td>latest version</td>
        </tr>
        <tr>
            <td>Opera</td>
            <td>latest version</td>
        </tr>
        <tr>
            <td>Tested email readers</td>
            <td>Outlook 2010, Outlook 2013, Lotus Notes 8.5, Gmail, Outlook 365</td>
        </tr>
        <tr>
            <td>HTTPS</td>
            <td>Only "Medium and High" ciphers are allowed (HIGH:MEDIUM:!ADH). TLSv1.x protocols are supported.</td>
        </tr>
        <tr>
            <td>Popup blocker for your URL</td>
            <td>Disabled</td>
        </tr>
    </tbody>
</table>

We systematically test the latest versions of Chrome, Firefox and Internet Explorer browsers to ensure the best experience for our users. Older versions of these browsers are not systematically tested, but run smoothly in most cases. If, however, there is a problem specific to a particular version of one of these browsers, please contact us.

### Tablet compatibility

CrossKnowledge LMS is compatible with iPad (2, 3, 4 and mini) - additional requirements may be needed for the content hosted on the LMS.

CrossKnowledge LMS is compatible with Android tablets (Chrome browser) - additional requirements may be needed for the content hosted on the LMS. 

### CrossKnowledge content additional requirements

As the contents are played on our LMS, you need the LMS requirements listed above, and the following ones:
 	
<table width="100%">
    <tbody>
        <tr>
            <td width="30%">Adobe Flash Player (CrossKnowledge Sessions)</td>
            <td width="70%">9.0.124 or higher</td>
        </tr>
        <tr>
            <td width="30%">PDF plugin</td>
            <td width="70%">Adobe Acrobat Reader (any version)</td>
        </tr>
        <tr>
            <td width="30%">Java (for Desktop contents)</td>
            <td width="70%">JVM 1.5 or higher</td>
        </tr>
    </tbody>
</table>

## Network Requirements

### Media extensions
The following media extensions should be authorised.<br/>
`.FLV, .mp3, .mp4, .srt, .woff, .vtt, .xhtml`

### Domain white-listing
The following domain names should be whitelisted.
```txt
http(s)://*.crossknowledge.com, http(s)://*.crossknowledge-player.com
```

If wildcards (*) are not allowed, authorise at least the following URLs:<br/>
#### General CKLS cloudfront URLs:

```txt
https://ckls-assets.crossknowledge.com/
https://ckls-api.crossknowledge.com/
https://ckls-cdn-eu.crossknowledge.com/
```

#### External medias (cloudfront URL)
```txt
https://d3d8qnlcu0b7xk.cloudfront.net
https://media-cdn2.crossknowledge.com
```

#### CK-Player URLs (for CrossKnowledge content delivery)

##### For users based in Europe
```txt
http(s)://cdn.crossknowledge.com/*
http(s)://d12yhdsdwe7din.cloudfront.net/* or http(s)://mohivecontents-eu.crossknowledge.com
```

##### For users based in the US:
```txt
rtmp://s11glde2jwx3y7.cloudfront.net/*
http(s)://d2niiguqm1v5wm.cloudfront.net/* or http(s)://ckcontents-na.crossknowledge.com
http(s)://dmi776hgmgo8n.cloudfront.net/* or http(s)://mohivecontents-na.crossknowledge.com
```

##### For users based in Asia:
```txt
rtmp://s2b3cf985zlt2f.cloudfront.net/*
http(s)://d8k70rs95pqqh.cloudfront.net/* or http(s)://ckcontents-jp.crossknowledge.com
http(s)://d14u2sk2qya69r.cloudfront.net/* or http(s)://mohivecontents-jp.crossknowledge.com
```

#### CKLM (XKA, Digital Literacy, Leaders...)
```txt
http(s)://d12pbbvc3h54xm.cloudfront.net/*
http(s)://cklm-prod.s3.amazonaws.com/*
https://cdn-cklm-prod.crossknowledge.com/*
https://ckcg.crossknowledge.com/*
```

#### CUSTOMER CONTENT CDN
```txt
https://ckls-cdn-eu.crossknowledge.com/*
https://ckls-cdn-na.crossknowledge.com/*
https://ckls-cdn-sa.crossknowledge.com/*
https://ckls-cdn-jp.crossknowledge.com/*
```

### AWS CloudFront IP Ranges

Part of our content is hosted on Amazon Cloud for a better experience around the globe.

```txt
54.182.0.0/16
54.192.0.0/16
54.230.0.0/16
54.239.128.0/18
54.239.192.0/19
54.240.128.0/18
204.246.164.0/22
204.246.168.0/22
204.246.174.0/23
204.246.176.0/20
205.251.192.0/19
205.251.249.0/24
205.251.250.0/23
205.251.252.0/23
205.251.254.0/24
216.137.32.0/19
```

### CKLS portal IPs addresses

##### Europe https://*.lms.crossknowledge.com:

```txt
Network range:
78.153.226.128/27

Load balancer: 78.153.226.153
```

##### Europe https://*.eu.crossknowledge.com: 

```txt
Network range :
78.153.234.128/26
```
<br/>
```txt
Load balancer: 78.153.234.185
```
<br/>
```txt
sftp server : sftp.crossknowledge.com (78.153.226.149)
sftp server : sftp.eu.crossknowledge.com (78.153.234.131)
Staging server : jnstaging.crossknowledge.com (78.153.226.147)
```
##### US
```txt
Could be any of the US-east-1 IP ranges listed in https://ip-ranges.amazonaws.com/ip-ranges.json Where  "service" = "EC2"
Load Balancer : 54.225.122.181 , 23.23.170.115
sftp server : sftp.na.crossknowledge.com (107.21.240.58) - until April 2017
sftp server : sftp.na.crossknowledge.com (54.221.219.193) - starting April 2017
```

##### South America:
```txt
Could be any of the sa-east-1 IP ranges listed in https://ip-ranges.amazonaws.com/ip-ranges.json Where  "service" = "EC2"
Load Balancer : 54.232.80.81 , 177.71.182.37
sftp server : sftp.sa.crossknowledge.com (54.232.80.112)
```
##### IPs addresses and URLs for CK-Hub:
```txt
46.51.186.229 or 54.228.234.84 May change, so you'd better use the a CNAME pointing to ck-hub.crossknowledge.com (also CNAME pointing to ck-hub-preprod.crossknowledge.com for UAT)
```

### Email servers requirements

##### Mail servers' IP addresses
```txt
85.31.192.42 ; 85.31.193.42 ; 85.31.193.7 ; 174.129.245.244
```

#### Hostnames of SMTP relay used for sending 	

```txt
smtp.jaguar-network.com
email-smtp.us-east-1.amazonaws.com
ses-smtp-prod-335357831.us-east-1.elb.amazonaws.com
smtp01.crossknowledge.com (EC2)
```
#### SPF records
You should also configure SPF records in your DNS domain zone(s) in order to allow CrossKnowledge to send emails on behalf of your email domain. [More about SPF.](http://www.openspf.org/SPF_Record_Syntax). <br/>

Add to the following to your existing SPF record:

```txt
include:mailrelay.crossknowledge.com
```

For informaiton, this actually corresponds to:
```txt
"v=spf1 mx ip4:85.31.192.42/32 ip4:85.31.193.42/32 ip4:85.31.193.7/32 ip4:174.129.245.244/32 include:amazonses.com -all"
```

## Sharepoint pre-requisites

### Sharepoint 2010
from IE7 to IE9, Firefox, Chrome
### Sharepoint 2013 
from IE8 to IE10, Firefox, Chrome<br/>

{% include note.html content="This plugin is not supported on the latest version of Office 365 (SharePoint 2016)." %}

## URL of CKLS platform
### Supported formats

* `https://customername.(eu lms na sa).crossknowledge.com`, with `http://customername.(eu-lms-na-sa).crossknowledge.com` being redirected to HTTPS (default setting).
* both `https://customername.(eu lms na sa).crossknowledge.com` and `http://customername.(eu-lms-na-sa).crossknowledge.com` without redirection from HTTP to HTTPS.
* `http://customername.customerdomain.com` as soon as customer domain contain a valid DNS entry that points to crossknowledge load balancer (NO HTTPS in this case).

### Unsupported formats
* `https://customername.customerdomain.com` - Crossknowledge only support HTTPS protocol with its own urls.

## My Learning App
My Learning is compatible with the following devices:

* Apple iOS: any device with iOS 10 and above (iPhone 5 and up, iPod 6 and up, iPad mini 2 or iPad 4 and up)
* Android: any device with Android KitKat 4.4 (API 19) - a non contractual list can be found (here)[http://www.theandroidcop.com/list-of-android-smartphones-and-tablets-getting-android-4-4-kitkat-update/]

## Learn App

Learn is an application for iPad and iPhone working on iOS 8 and up. An Android application also exists (Android 4.2+). 

### Learning objects compatibility online and offline mode

Find below the list of learning objects with their compatibility status with Learn application (this list is subject to change).


Learning object type | Online mode | Offline mode
---- | ---- | ----
Custom SCORM | yes (monosco) | yes
Mohive| yes | yes
Easyquizz | no | no
Image | no | no
Audio mp3 | yes | yes
Video | yes | yes
Pdf | yes | yes
PPT | no | no
Text page | no | no
Zip file | no | no
YouTube | no | no
Slideshare | no | no
Brightcove | no | no
URL | no | no
Digital Literacy | yes | yes
Leaders Videocast | yes | yes
Business Digest | yes | soon
CrossKnowledge Essentials | yes | yes
CrossKnowledge Action Tips | yes | yes
CrossKnowledge Sessions V3 & The team | yes | yes 