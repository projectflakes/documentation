=====
Adyen
=====

Connecting an **Adyen payment terminal** allows you to offer a fluid payment flow to your customers
and ease the work of your cashiers.

Configuration
=============

Start by creating your Adyen account on `Adyen's website <https://www.adyen.com/>`_. Then, board
your terminal following the steps described on your terminal's screen.

.. tip::
   In case of doubt, please refer to `Adyen's documentation.
   <https://docs.adyen.com/point-of-sale/user-manuals_>`_

Configure the payment method
----------------------------

First, go to :menuselection:`Pos App --> Configuration --> Settings`, and enable :guilabel:`Adyen`
under the :guilabel:`Payment Terminals` section.

Then, go to :menuselection:`Configuration --> Payment Methods` and create a new payment method.
Select :guilabel:`Adyen` in the :guilabel:`Use a Payment Terminal` field.

.. note::
   The selected journal **must** be a bank journal for the :guilabel:`Use a payment terminal` field
   to appear.

Finally, fill the the mandatory fields with an :guilabel:`Adyen API key`, and an :guilabel:`Adyen
Terminal Identifier`.

.. tabs::

   .. tab:: Adyen API key

      The **Adyen API key** is a key used to authenticate your requests. To generate an API key, go
      to your **Adyen account**.

      Then, go to :menuselection:`Developers --> API credentials`. Create a new credential or click
      on an existing one.

      Click on :guilabel:`Generate an API key` and copy-paste that key onto the Odoo mandatory
      field.      .

      .. tip::
         In case of doubt, please refer to `Adyen's documentation.
         <https://docs.adyen.com/development-resources/api-credentials#generate-api-key_>`_

   .. tab:: Adyen terminal identifier

      The **Adyen Terminal Identifier** is your terminal's serial number, which is used to identify
      the hardware.

      To find this number, go to your **Adyen account**. Then, go to :menuselection:`Point of Sale
      --> Terminals`, select the terminal to link, and copy-paste its serial number onto the Odoo
      mandatory field.

Add a new payment method to the pos
===================================

To add a new payment method to a **point of sale**, go to :menuselection:`pos settings --> Payments
--> Payment Methods`, add your new method for Adyen, and save.

Pay with a payment terminal
===========================
When processing a payment, select :guilabel:`Adyen` as payment method. Check the amount and click on
:guilabel:`Send`. Once the payment is successful, the status changes to :guilabel:`Payment
Successful`.

.. note::
   * In case of connexion issues between Odoo and the payment terminal, force the payment by
     clicking on *Force Done*, which allows you to validate the order.
     This option is only available after receiving an error message informing you that the
     connection failed.
   * To cancel the payment request, click on **cancel**.