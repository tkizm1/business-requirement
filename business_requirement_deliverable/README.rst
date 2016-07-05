.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
   :target: https://www.gnu.org/licenses/agpl-3.0-standalone.html
   :alt: License: AGPL-3

================================
Business Requirement Deliverable
================================

Introduction
^^^^^^^^^^^^

This module is part of a set ("Business Requirement").
The Business Requirements features start as independent entities, and can be 
used as standalone.

Additional modules integrate them with other business areas, such as Sales, 
Procurement, Project or Analytic Accounting. For example:

* Sales Quotation can have an estimation supported by a BR analysis
* Project Tasks can be related to the BRs they implement or support
* Procurement and purchase can be generated out of the BR


|image7|

.. |image7| image:: business_requirement_deliverable/static/img/bus_req_tree.png
   :width: 800 px
   :alt: Business Requirement List view

The following diagram gives a simplified view of the universe:

|image11|

.. |image11| image:: business_requirement_deliverable/static/img/bus_req_module_diag.png
   :width: 800 px
   :alt: Business Requirement modules diagram

What is a Business Requirement?
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

A Business requirement (BR) is the expression of a business need by a customer 
or internal project user.
A BR can contain multiple different parts depending on the company needs:

* Customer Story: this is the requirement as expressed by the customer
* Scenario: How/where the current solution can provide a suitable scenario to 
  answer the customer story
* Gap: For the uncovered part of the scenario, elaborate the gap/need for specific 
  developments/setup
* Deliverables to be provided to the customer/user
* Resources necessary to achieve the deliverables
* Additional information (approval, cost control etc.)

These modules were originally designed for the service/IT industry but the 
requirement management is generic and can apply to many cases/industries (customer 
or internal projects):

* Construction
* Trading (New product development)
* Business Consultancy
* IT development

What is the difference between a BR and CRM lead?

* CRM leads are sales oriented
* BR are project and workload estimation oriented

How to use this module?
^^^^^^^^^^^^^^^^^^^^^^^

This module introduces 2 main concepts in the business requirements model:

* Deliverable lines
* Resource lines

What is a Deliverable Line?

Deliverable Lines (DL) contains products and services that we will deliver to the 
customer. They are **customer oriented** and can be either physical or service products

* Servers and procured goods
* Gap analysis services
* Module development services
* Training etc.

DL directly depends on the BR.

|image0|

.. |image0| image:: business_requirement_deliverable/static/img/bus_req_deliverable.png
   :width: 800 px
   :alt: Business Requirement Deliverable lines


What are Resources Lines?

Resources Lines (RL) are the different tasks or procurements needed to achieve one deliverable:

* Service tasks (Development, consultant etc.)
* Procurement of other physical goods (server, etc.)
* Procurement of other virtual goods (templates, sub-contracting, etc.)

RL directly depends on the DL.


|image1|

.. |image1| image:: business_requirement_deliverable/static/img/bus_req_resource.png
   :width: 800 px
   :alt: Business Requirement Resources lines

What is the difference between Deliverable and Resources?

Deliverables are:

* provided to the customer (“Functioning Website”)
* Valued at Customer Sales Price
* Used in Sales Quotations

Resources are:

* executed internally (“Server+CSS modifications”)
* Valued at Cost Price
* Used in Project management or procurement management

Example
^^^^^^^
* BR1

  * DL1

    * RL1
    * RL2
    * RL3

  * DL2

    * RL4
    * RL5
    * RL6

* BR2

  * DL3

    * RL7
    * RL8

  * DL4

    * RL9


Installation
============

No specific steps required

Configuration
=============

Users
^^^^^

No specific ACL are required for the module.

Master project
^^^^^^^^^^^^^^

You can define a master project linked to the business requirement.

You have to specify a estimation price list in the master project, used for 
deliverable price management. If no pricelist is specified in the project, 
the one from the customer associated will be used.


Usage
=====

#. In the BR, you can add as many deliverable lines as necessary. Price of the deliverable lines will depend on the pricelist in master project or customer.

#. Once the deliverable lines are created you can create as many resources lines as necessary in each DL. Cost price of the product will apply

#. in RL you can already assign the responsible of the task if necessary

|image2|

.. |image2| image:: business_requirement_deliverable/static/img/bus_req_deliverable2.png
   :width: 800 px
   :alt: Inputing the deliverables and resources lines


.. image:: https://odoo-community.org/website/image/ir.attachment/5784_f2813bd/datas
   :alt: Try me on Runbot
   :target: https://runbot.odoo-community.org/runbot/140/8.0


Bug Tracker
===========

Bugs are tracked on `GitHub Issues <https://github.com/OCA/business-requirement/issues>`_.
In case of trouble, please check there if your issue has already been reported.
If you spotted it first, help us smashing it by providing a detailed and welcomed feedback.

Credits
=======

Contributors
------------

* Eric Caudal <eric.caudal@elico-corp.com>
* Alex Duan <alex.duan@elico-corp.com>
* Xie XiaoPeng <xie.xiaopeng@elico-corp.com>
* Victor M. Martin <victor.martin@elico-corp.com>

Maintainer
----------

.. image:: https://odoo-community.org/logo.png
   :alt: Odoo Community Association
   :target: https://odoo-community.org

This module is maintained by the OCA.

OCA, or the Odoo Community Association, is a nonprofit organization whose
mission is to support the collaborative development of Odoo features and
promote its widespread use.

To contribute to this module, please visit https://odoo-community.org.