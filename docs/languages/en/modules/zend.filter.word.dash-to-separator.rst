.. _zend.filter.set.dashtoseparator:

Word\\DashToSeparator
---------------------

This filter modifies a given string such that 'words-with-dashes' are converted to 'words with dashes'.

.. _zend.filter.set.dashtoseparator.options:

Supported options for Zend\\Filter\\Word\\DashToSeparator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

The following options are supported for ``Zend\Filter\Word\DashToSeparator``:

- **separator**: A separator char. If this is not set the separator will be a space character.

.. _zend.filter.set.dashtoseparator.basic:

Basic usage
^^^^^^^^^^^

A basic example of usage is below:

.. code-block:: php
   :linenos:

   $filter = new Zend\Filter\Word\DashToSeparator('+');
   // or new Zend\Filter\Word\CamelCaseToSeparator(array('separator' => '+'));

   print $filter->filter('this-is-my-content');

The above example returns 'this+is+my+content'.

Default behaviour for Zend\\Filter\\Word\\DashToSeparator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

.. code-block:: php
   :linenos:

   $filter = new Zend\Filter\Word\DashToSeparator();

   print $filter->filter('this-is-my-content');

The above example returns 'this is my content'.

