==================
Partner auto match
==================

.. 
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! source digest: sha256:ed308cc7c36b0d08c33cf3cd62653ea7d72077bb59ead1bed978c26e22d8f812
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-CompassionCH%2Fcompassion--modules-lightgray.png?logo=github
    :target: https://github.com/CompassionCH/compassion-modules/tree/14.0/partner_auto_match
    :alt: CompassionCH/compassion-modules

|badge1| |badge2| |badge3|

This module doesn't do anything on its own, but enables other modules to
find and update or create partner given any field data.

**Table of contents**

.. contents::
   :local:

Usage
=====

To use this module, you need to:

-  Inherit the module
-  Use *self.env["res.partner.match"].match_values_to_partner(vals)*
   method in order to match partner given some partner data dictionary.
-  Inherit *\_process_create_infos* method if you want to customize
   partner creation (in case of match fail)
-  Inherit *\_process_update_vals* method if you want to customize
   partner update (in case of match success)
-  Inherit *\_match_get_rules_order* in order to alter match rules
   order, or to add remove any rule
-  Add a method *\_match\_<rule_name>* in order to add a new match rule
-  Inherit *\_get_valid_create_fields* to restrict/extend fields allowed
   for partner creation.
-  Inherit *\_get_valid_update_fields* to restrict/extend fields allowed
   for partner update.

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/CompassionCH/compassion-modules/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us to smash it by providing a detailed and welcomed
`feedback <https://github.com/CompassionCH/compassion-modules/issues/new?body=module:%20partner_auto_match%0Aversion:%2014.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
-------

* Compassion Switzerland

Contributors
------------

-  Emanuel Cino <ecino@compassion.ch>

Maintainers
-----------

.. |maintainer-ecino| image:: https://github.com/ecino.png?size=40px
    :target: https://github.com/ecino
    :alt: ecino

Current maintainer:

|maintainer-ecino| 

This module is part of the `CompassionCH/compassion-modules <https://github.com/CompassionCH/compassion-modules/tree/14.0/partner_auto_match>`_ project on GitHub.

You are welcome to contribute.
