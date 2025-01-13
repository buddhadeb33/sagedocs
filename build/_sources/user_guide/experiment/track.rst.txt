.. _end_tail_imputer:

.. currentmodule:: feature_engine.imputation

Tracking and Managing Experiments
=================================

Tracking and Managing Experiments:
Searching and Sorting
Viewing Metrics and Logs







Note that after the imputation, if the percentage of missing values is relatively big,
the variable distribution will differ from the original one (in red the imputed
variable):

.. code:: python

	fig = plt.figure()
	ax = fig.add_subplot(111)
	X_train['LotFrontage'].plot(kind='kde', ax=ax)
	train_t['LotFrontage'].plot(kind='kde', ax=ax, color='red')
	lines, labels = ax.get_legend_handles_labels()
	ax.legend(lines, labels, loc='best')

.. image:: ../../images/endtailimputer.png

Additional resources
--------------------

In the following Jupyter notebook you will find more details on the functionality of the
:class:`CategoricalImputer()`, including how to select numerical variables automatically,
how to impute with the most frequent category, and how to impute with a used defined
string.

- `Jupyter notebook <https://nbviewer.org/github/feature-engine/feature-engine-examples/blob/main/imputation/EndTailImputer.ipynb>`_

For more details about this and other feature engineering methods check out these resources:


.. figure::  ../../images/feml.png
   :width: 300
   :figclass: align-center
   :align: left
   :target: https://www.trainindata.com/p/feature-engineering-for-machine-learning

   Feature Engineering for Machine Learning

|
|
|
|
|
|
|
|
|
|

Or read our book:

.. figure::  ../../images/cookbook.png
   :width: 200
   :figclass: align-center
   :align: left
   :target: https://www.packtpub.com/en-us/product/python-feature-engineering-cookbook-9781835883587

   Python Feature Engineering Cookbook

|
|
|
|
|
|
|
|
|
|
|
|
|

Both our book and course are suitable for beginners and more advanced data scientists
alike. By purchasing them you are supporting Sole, the main developer of Feature-engine.