.. include:: /Includes.rst.txt
.. _columns-properties-exclude:

=======
exclude
=======

.. confval:: exclude

   :Path: $GLOBALS['TCA'][$table]['columns'][$field]
   :Required: false
   :type: boolean
   :Scope: Proc. / Display

   If set, all backend users are prevented from editing the field unless they
   are members of a backend user group with this field added as an
   "Allowed Excludefield" (or "admin" user).

   See :ref:`Access lists <t3coreapi:access-options-access-lists>` for more
   about permissions.

Example
=======

Simple input field
------------------

.. code-block:: php

   [
       'columns' => [
           'input_2' => [
               'label' => 'input_2 description',
               'exclude' => true,
               'config' => [
                   'type' => 'input',
                   
               ],
           ],
       ],
   ]
