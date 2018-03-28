Webform Clear Module
============================

Clears specific Webforms from the database after a selected period 
(immediately upon submission or 1,7,30, 60, 90, 365 days).
Any uploaded files associated to the Webform will also be
deleted.

This can happen either never, immediately, or after a selected
period. A default value for the clearing period can be set both site
wide basis, and per Webform.

PREREQUISITES
-------------
Webform module

INSTALLATION
------------
Install this module using the official Backdrop CMS instructions at
  https://backdropcms.org/guide/modules

CONFIGURATION
-------------
. The "Set Webform submission storage periods" permission can be set at
  'admin/config/people/permissions/ROLE'
  
. Go to "admin/config/content/webform_clear" if you want to change
   the default storage period for Webforms to something other than "Do
   not delete".

   Submissions to any Webforms created/edited before changing this
   default value will not be affected. Submissions to any Webforms
   created after changing this default value will be affected.

. In the "Form settings" for a Webform ('node/NODE ID/webform/configure'),
   this value can be overriden by users with the "Set up Webform
   submission storage periods" permission.

   For other users, this dropdown will be disabled (grayed out) and be
   set to whatever it was set to by another user, or to the default
   value.

Current Maintainer
------------------
- Jörg Kienitz (https://github.com/vtad)

Credits
-------
- Port of https://www.drupal.org/project/webform_clear/releases/7.x-2.x-dev
  updated 12 Nov 2017
- Originally written for Drupal by
Robert Castelo (http://www.codepositive.com/)


License
-------
This project is GPL v2 software. See the LICENSE.txt file in this directory for
complete text.