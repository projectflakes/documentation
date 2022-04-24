=============================================================
Digitalize documents with optical character recognition (OCR)
=============================================================

Encoding vendor bills or customer invoices manually is a time-consuming task. With optical character
recognition (OCR), digitalize and import these documents automatically into your database.

.. seealso::
   - Odoo Tutorials: OCR (link to the new video - not ready yet)
   - `Try it out <https://www.odoo.com/app/invoice-automation>`_! Upload one of your bills or try
     one of our samples to see how it works.
   - :doc:`/applications/general/in_app_purchase`

Configuration
=============

Digitalization is an :doc:`In-App Purchase (IAP) </applications/general/in_app_purchase>` service
that requires prepaid credits to work. To buy credits, go to :menuselection:`Accounting -->
Configuration --> Settings --> Digitization` and click on :guilabel:`Buy credits`. Or go to
:menuselection:`General Settings --> Contacts` and under :guilabel:`Odoo IAP` click on
:guilabel:`View My Services`.

.. note::
   - If you are on Odoo Online (SAAS) and have the Enterprise version, you benefit from free trial
     credits to test the feature.

In :menuselection:`Accounting --> Configuration --> Settings --> Digitization`, choose whether the
:guilabel:`Vendor Bills` and :guilabel:`Customer Invoices` should be processed automatically (with
OCR) or manually (on demand).

The :guilabel:`single Invoice Line Per Tax` option can also be selected. It enables to get only one
line created per tax in the new bill, regardless of the number of lines from the invoice.

Digitalizing vendor bills
=========================

Your :guilabel:`Vendor Bills` can be uploaded from the :guilabel:`Accounting Dashboard` or by going
to  :menuselection:`Accounting --> Vendors -->  Bills`. Based on your configuration, it either
processes the documents automatically, or you need to click on :guilabel:`Send for digitalization`
to do it manually.

Digitalizing customer invoices
==============================

From the :guilabel:`Accounting Dashboard`, select the extra menu field ⋮ in the :guilabel:`Customer
Invoices` journal, and select :guilabel:`Upload Invoices`. Or go to :menuselection:`Accounting -->
Customers --> Invoices` and select :guilabel:`Upload`.

.. note::
   - The more documents you scan, the better the system identifies the correct data.
   - If the document you upload contains several bills, the OCR detects them automatically and the
     Documents App can split them all.
   - You can also create and upload your documents from the Documents App.
   - Once the data is extracted from the PDF, you can correct it if necessary by clicking on the
     respective tag (available in Edit mode) and selecting the proper information instead.