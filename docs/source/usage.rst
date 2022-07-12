Usage
=====

.. _installation:

Installation
------------

To use simsep, first install it using pip:

.. code-block:: console

   (.venv) $ pip install simsep

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``simsep.get_random_ingredients()`` function:

.. autofunction:: simsep.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`simsep.get_random_ingredients`
will raise an exception.

.. autoexception:: simsep.InvalidKindError

For example:

>>> import simsep
>>> simsep.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

