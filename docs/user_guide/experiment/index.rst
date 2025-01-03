.. -*- mode: rst -*-

Experiment
=======================
AWS SageMaker Experiment is that it allows you to automatically capture and store every single metric and artifact from your model training runs, even across multiple experiments. This feature makes it easy to visualize how changes in hyperparameters or data affect model performance over time. It also simplifies comparisons of different experiment runs, enabling data scientists to efficiently identify trends, best-performing models, and areas for improvement, all without manually tracking this information. This level of automation and detail in experimentation is a huge time-saver and can significantly enhance model optimization.

.. figure::  ../../images/sagemaker_experiment.png
   :align:   center

|


Experiment
~~~~~~~~~~~

.. toctree::
   :maxdepth: 1

   overview
   experiment_setup
   track
   api
   trial
   logging_metrics
   troubleshoot