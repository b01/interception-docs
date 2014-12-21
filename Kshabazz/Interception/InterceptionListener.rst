--------------------------------------------
Kshabazz\\Interception\\InterceptionListener
--------------------------------------------

.. php:namespace: Kshabazz\\Interception

.. php:class:: InterceptionListener

    Class InterceptionListener

    .. php:method:: __construct($pWrapperClass, $pSaveDir = NULL, $pWrappers = NULL)

        :type $pWrapperClass: string
        :param $pWrapperClass: Interception stream wrapper to register.
        :type $pSaveDir: string
        :param $pSaveDir: Directory where RSD files will be saved.
        :param $pWrappers:

    .. php:method:: endTestSuite(PHPUnit_Framework_TestSuite $suite)

        Restore PHP built-in HTTP stream wrapper and perform any other clean-up.

        :type $suite: PHPUnit_Framework_TestSuite
        :param $suite:
        :returns: bool

    .. php:method:: startTest(PHPUnit_Framework_Test $test)

        :type $test: PHPUnit_Framework_Test
        :param $test:

    .. php:method:: startTestSuite(PHPUnit_Framework_TestSuite $suite)

        :type $suite: PHPUnit_Framework_TestSuite
        :param $suite:
