To install on your server for the following commands after changing to your web directory:

git clone https://github.com/campaignkings/webphone.git

chmod -R 744 webphone

chown -R apache:apache webphone

# CampaignKings-3.2.5

Version 3.2.5
With this release comes the following improvements:

A complete rewrite of the core CampaignKings Webphone code to support SIP.js v0.20.1
This does require 'rtcp_mux=yes' be set in the template you are using for your webphone
Support for passing a settings container from ViciDial to Ckwebphone to allow additional settings to be added in the future without ViciDial changes
Added the ability to enable/disable various browser audio processing like Echo Cancellation and Automatic Gain Control
Does require the Ckwebphone settings container support in Ckwebphone
Auto call agent conference on successful registration. This is similar to a feature that was added to some forks of Ckwebphone but it will work even if Ckphone and ViciDial are hosted on different domains.
