.. include:: /Includes.rst.txt
.. _columns-radio-properties-items:

=====
items
=====

.. confval:: items (type => radio)

   :Path: $GLOBALS['TCA'][$table]['columns'][$field]['config']
   :required: true
   :type: array
   :Scope: Display  / Proc.

   An array of values which can be selected.

   Each entry is in itself an array where the  *first entry* is the displayed *title* (string or LLL reference)
   and the *second entry* is the *value* of the field in database if that radio is selected. Values can be
   integer numbers or string values.
