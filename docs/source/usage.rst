Usage
=====

.. _installation:

Installation
------------

To use Fandao, first install it using pip:

.. code-block:: console

   (.venv) $ pip install afandao

Creating recipes
----------------

To retrieve a list of random ingredients,
you can use the ``fandao.get_random_ingredients()`` function:

.. autofunction:: fandao.get_random_ingredients

The ``kind`` parameter should be either ``"meat"``, ``"fish"``,
or ``"veggies"``. Otherwise, :py:func:`fandao.get_random_ingredients`
will raise an exception.

.. autoexception:: fandao.InvalidKindError

For example:

>>> import fandao
>>> fandao.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

