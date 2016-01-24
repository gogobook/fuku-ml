Perceptron Binary Classification Learning Algorithm
============

Run demo dataset: Basic Naive Cycle PLA
-----------------

.. code-block:: py

    >>> import numpy as np

    >>> import FukuML.PLA as pla

    >>> pla_bc = pla.BinaryClassifier()

    >>> pla_bc.load_train_data()

    >>> pla_bc.init_W()

    >>> pla_bc.train()

    >>> test_data = '0.97681 0.10723 0.64385 0.29556 1'

    >>> prediction = pla_bc.prediction(test_data)

    >>> future_data = '0.97681 0.10723 0.64385 0.29556'

    >>> prediction = pla_bc.prediction(future_data, 'future_data')

Run demo dataset: Random Cycle PLA
-----------------

.. code-block:: py

    >>> import numpy as np

    >>> import FukuML.PLA as pla

    >>> pla_bc = pla.BinaryClassifier()

    >>> pla_bc.load_train_data()

    >>> pla_bc.init_W()

    >>> pla_bc.train('random')

    >>> test_data = '0.97681 0.10723 0.64385 0.29556 1'

    >>> prediction = pla_bc.prediction(test_data)

    >>> future_data = '0.97681 0.10723 0.64385 0.29556'

    >>> prediction = pla_bc.prediction(future_data, 'future_data')

Run demo dataset: Random Cycle PLA alpha=0.5 step correction
-----------------

.. code-block:: py

    >>> import numpy as np

    >>> import FukuML.PLA as pla

    >>> pla_bc = pla.BinaryClassifier()

    >>> pla_bc.load_train_data()

    >>> pla_bc.init_W()

    >>> pla_bc.train('random', 0.5)

    >>> test_data = '0.97681 0.10723 0.64385 0.29556 1'

    >>> prediction = pla_bc.prediction(test_data)

    >>> future_data = '0.97681 0.10723 0.64385 0.29556'

    >>> prediction = pla_bc.prediction(future_data, 'future_data')

Pocket Perceptron Binary Classification Learning Algorithm
============

Run demo dataset
-----------------

.. code-block:: py

    >>> import numpy as np

    >>> import FukuML.PocketPLA as pocket

    >>> pocket_bc = pocket.BinaryClassifier()

    >>> pocket_bc.load_train_data()

    >>> pocket_bc.init_W()

    >>> W = pocket_bc.train(50)

    >>> test_data = '0.62771 0.11513 0.82235 0.14493 -1'

    >>> prediction = pocket_bc.prediction(test_data)

    >>> future_data = '0.62771 0.11513 0.82235 0.14493'

    >>> prediction = pocket_bc.prediction(future_data, 'future_data')

    >>> pocket_bc.load_test_data()

    >>> pocket_bc.calculate_avg_error(pocket_bc.test_X, pocket_bc.test_Y, W)

Linear Regression Learning Algorithm
============

Run demo dataset
-----------------

.. code-block:: py

    >>> import numpy as np

    >>> import FukuML.LinearRegression as linear_regression

    >>> linear = linear_regression.LinearRegression()

    >>> linear.load_train_data()

    >>> linear.init_W()

    >>> W = linear.train()

    >>> test_data = '0.62771 0.11513 0.82235 0.14493 -1'

    >>> prediction = linear.prediction(test_data)

    >>> future_data = '0.62771 0.11513 0.82235 0.14493'

    >>> prediction = linear.prediction(future_data, 'future_data')

    >>> linear.load_test_data()

    >>> linear.calculate_avg_error(linear.test_X, linear.test_Y, W)

Linear Regression Binary Classification Learning Algorithm
============

Run demo dataset
-----------------

.. code-block:: py

    >>> import numpy as np

    >>> import FukuML.LinearRegression as linear_regression

    >>> linear_bc = linear_regression.BinaryClassifier()

    >>> linear_bc.load_train_data()

    >>> linear_bc.init_W()

    >>> W = linear_bc.train()

    >>> test_data = '0.62771 0.11513 0.82235 0.14493 -1'

    >>> prediction = linear_bc.prediction(test_data)

    >>> future_data = '0.62771 0.11513 0.82235 0.14493'

    >>> prediction = linear_bc.prediction(future_data, 'future_data')

    >>> linear_bc.load_test_data()

    >>> linear_bc.calculate_avg_error(linear_bc.test_X, linear_bc.test_Y, W)