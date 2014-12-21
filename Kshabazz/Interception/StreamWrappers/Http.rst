--------------------------------------------
Kshabazz\\Interception\\StreamWrappers\\Http
--------------------------------------------

.. php:namespace: Kshabazz\\Interception\\StreamWrappers

.. php:class:: Http

    Class Http

    .. php:const:: RESOURCE_TYPE_FILE

    .. php:const:: RESOURCE_TYPE_SOCKET

    .. php:attr:: context

        resource

    .. php:attr:: position

        int

    .. php:method:: __construct()

        Constructor

    .. php:method:: count()

    .. php:method:: offsetExists($pKey)

        Allow access via indices.

        :type $pKey: mixed
        :param $pKey:
        :returns: bool

    .. php:method:: offsetGet($pKey)

        :param $pKey:

    .. php:method:: offsetSet($pKey, $pValue)

        :param $pKey:
        :param $pValue:

    .. php:method:: offsetUnset($pKey)

        :type $pKey: mixed
        :param $pKey:

    .. php:method:: stream_close()

        Close the resource.

        :returns: void

    .. php:method:: stream_eof()

        :returns: bool

    .. php:method:: stream_open($pPath, $pMode, $pFlags, $pOpenedPath)

        Open a stream resource.

        :type $pPath: string
        :param $pPath:
        :type $pMode: string
        :param $pMode:
        :type $pFlags: int
        :param $pFlags:
        :type $pOpenedPath: string
        :param $pOpenedPath:
        :returns: bool

    .. php:method:: stream_read($count)

        :type $count: int
        :param $count:
        :returns: string

    .. php:method:: stream_stat()

        TODO: Find out why this is trigger when using \file_get_contents().

        :returns: array

    .. php:method:: clearPersistSaveFile()

        Clear the persist save filename.

        :returns: bool TRUE when save file is cleared.

    .. php:method:: clearSaveFile()

        Clear the save file name.

        :returns: bool TRUE when save file is cleared, FALSE when $saveFilePersist is TRUE.

    .. php:method:: getSaveDir()

        Get directory where to save raw socket data files.

        :returns: string

    .. php:method:: getSaveFilename()

        Get save file name.

        :returns: string

    .. php:method:: persistSaveFile($pPersistFilename)

        Allow the save file name to persist, until called with FALSE.

        :type $pPersistFilename: string
        :param $pPersistFilename:
        :returns: bool Current setting.

    .. php:method:: persistSuffix()

        Add a suffix to the file to prevent overwriting when persisting save file.

        :returns: string

    .. php:method:: setSaveDir($pDirectory)

        Set directory to save socket data files.

        :param $pDirectory:
        :returns: bool

    .. php:method:: setSaveFilename($pFilename)

        Set the file name for the local file.

        :param $pFilename:
        :returns: bool

    .. php:method:: isValidFilename($pFilename)

        Validate a name filename.

        :param $pFilename:
        :returns: bool

    .. php:method:: buildRequest()

        Build the request according to:
        http://www.w3.org/Protocols/rfc2616/rfc2616-sec5.html

    .. php:method:: getSaveFile()

        Get the full file path by generating one from the URL, or the one set by
        the developer.

        :returns: bool

    .. php:method:: populateResponseHeaders()

        Parse the content for the headers.

    .. php:method:: readFromSocket($pResource, $pLength = 100)

        :type $pResource: resource
        :param $pResource:
        :type $pLength: int
        :param $pLength:
        :returns: bool

    .. php:method:: readFromResource($pCount = 100)

        :type $pCount: int
        :param $pCount:
        :returns: bool|string

    .. php:method:: triggerSocketError()

        Trigger socket error.
