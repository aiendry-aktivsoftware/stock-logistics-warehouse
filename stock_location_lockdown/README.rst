=======================
Stock Location Lockdown
=======================

.. !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
   !! This file is generated by oca-gen-addon-readme !!
   !! changes will be overwritten.                   !!
   !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!

.. |badge1| image:: https://img.shields.io/badge/maturity-Beta-yellow.png
    :target: https://odoo-community.org/page/development-status
    :alt: Beta
.. |badge2| image:: https://img.shields.io/badge/licence-AGPL--3-blue.png
    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
    :alt: License: AGPL-3
.. |badge3| image:: https://img.shields.io/badge/github-OCA%2Fstock--logistics--warehouse-lightgray.png?logo=github
    :target: https://github.com/OCA/stock-logistics-warehouse/tree/16.0/stock_location_lockdown
    :alt: OCA/stock-logistics-warehouse
.. |badge4| image:: https://img.shields.io/badge/weblate-Translate%20me-F47D42.png
    :target: https://translation.odoo-community.org/projects/stock-logistics-warehouse-16-0/stock-logistics-warehouse-16-0-stock_location_lockdown
    :alt: Translate me on Weblate
.. |badge5| image:: https://img.shields.io/badge/runbot-Try%20me-875A7B.png
    :target: https://runbot.odoo-community.org/runbot/153/16.0
    :alt: Try me on Runbot

|badge1| |badge2| |badge3| |badge4| |badge5| 

The aim of this module is to mark internal locations where no product should transit.
Indeed, in complex warehouse setups, we may have a complicated tree of internal locations with parent locations only used to create the hierarchy of the internal locations.
We may want to avoid to put stock on these parent internal locations since they are not physical locations, they just represent a zone of the warehouse.
Theses locations must have *Location Type* set to *Internal Location* because they belong to a warehouse (they can't be configured with *Location Type* set to *View*, cf `Odoo bug #26679 <https://github.com/odoo/odoo/issues/26679>`_). With this module, you will be able to enable a new option *Block stock entrance* for these locations.

**Table of contents**

.. contents::
   :local:

Usage
=====

* Once the module is installed, select any internal location for which you want to prevent stock entrance and check the box *Block Stock Entrance*. Then, you won't be allow to add stock on these locations.

Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/stock-logistics-warehouse/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed
`feedback <https://github.com/OCA/stock-logistics-warehouse/issues/new?body=module:%20stock_location_lockdown%0Aversion:%2016.0%0A%0A**Steps%20to%20reproduce**%0A-%20...%0A%0A**Current%20behavior**%0A%0A**Expected%20behavior**>`_.

Do not contact contributors directly about support or help with technical issues.

Credits
=======

Authors
~~~~~~~

* Akretion

Contributors
~~~~~~~~~~~~

* Florian da Costa <florian.dacosta@akretion.com>
* David Montull Guasch <david.montull@bt-group.com>
* Urvisha Desai <udesai@opensourceintegrators.com>

Maintainers
~~~~~~~~~~~

This module is maintained by the OCA.

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

This module is part of the `OCA/stock-logistics-warehouse <https://github.com/OCA/stock-logistics-warehouse/tree/16.0/stock_location_lockdown>`_ project on GitHub.

You are welcome to contribute. To learn how please visit https://odoo-community.org/page/Contribute.
