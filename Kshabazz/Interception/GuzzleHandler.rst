-------------------------------------
Kshabazz\\Interception\\GuzzleHandler
-------------------------------------

.. php:namespace: Kshabazz\\Interception

.. php:class:: GuzzleHandler

    Class GuzzleHandler

    .. php:method:: __construct($options = [])

        :param $options:

    .. php:method:: __invoke($request)

        :param $request:

    .. php:method:: createResponse($request, $url, $hdrs, $stream)

        :param $request:
        :param $url:
        :param $hdrs:
        :param $stream:

    .. php:method:: checkDecode($request, $response, $stream)

        :param $request:
        :param $response:
        :param $stream:

    .. php:method:: drain($stream, $dest)

        Drains the stream into the "save_to" client option.

        :param $stream:
        :type $dest: string|resource|StreamInterface
        :param $dest:
        :returns: Stream

    .. php:method:: createErrorResponse($url, RingException $e)

        Creates an error response for the given stream.

        :param $url:
        :type $e: RingException
        :param $e:
        :returns: array

    .. php:method:: createResource($callback)

        Create a resource and check to ensure it was created successfully

        :type $callback: callable
        :param $callback: Callable that returns stream resource
        :returns: resource

    .. php:method:: createStream($url, $request, $http_response_header)

        :param $url:
        :param $request:
        :param $http_response_header:

    .. php:method:: getDefaultOptions($request)

        :param $request:

    .. php:method:: add_proxy($request, $options, $value, $params)

        :param $request:
        :param $options:
        :param $value:
        :param $params:

    .. php:method:: add_timeout($request, $options, $value, $params)

        :param $request:
        :param $options:
        :param $value:
        :param $params:

    .. php:method:: add_verify($request, $options, $value, $params)

        :param $request:
        :param $options:
        :param $value:
        :param $params:

    .. php:method:: add_cert($request, $options, $value, $params)

        :param $request:
        :param $options:
        :param $value:
        :param $params:

    .. php:method:: add_progress($request, $options, $value, $params)

        :param $request:
        :param $options:
        :param $value:
        :param $params:

    .. php:method:: add_debug($request, $options, $value, $params)

        :param $request:
        :param $options:
        :param $value:
        :param $params:

    .. php:method:: applyCustomOptions($request, $options)

        :param $request:
        :param $options:

    .. php:method:: createContext($request, $options, $params)

        :param $request:
        :param $options:
        :param $params:

    .. php:method:: createStreamResource($url, $request, $options, $context, $http_response_header)

        :param $url:
        :param $request:
        :param $options:
        :param $context:
        :param $http_response_header:
