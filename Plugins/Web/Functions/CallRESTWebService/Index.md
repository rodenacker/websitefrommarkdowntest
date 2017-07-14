CallRESTWebService
==================

The CallRESTWebService function allows for calling a REST web service.

This function can be used to call other published Linx processes on the
same or different Linx servers.

Properties
----------

-  #### Type

    The type of authentication configured on the server for the web
    service being called. Most common is *Basic*.

-  #### Domain

    The domain to authenticate the user against.

-  #### Username

    The username to authenticate against.

-  #### Password

    The password to authenticate against.

-  #### Method{#properties-method}

    Most web services are configured to accept messages using GET or
    POST. Some may also use HEAD, PUT or DELETE.

-  #### Timeout

    The timeout value for the web service call.

-  #### URL

    The base URL to use for the service request. This excludes any
    parameter-specific information that are send with the request. A
    valid example for this field could look like this:  
    *http://localhost:8022/Service/ExecuteService*

-  #### Query string

    A list of parameters to use in order to build up the query string. A
    query string with a format similar to the following will be
    generated (note that parameters have not been URL encoded to improve
    readability):  
     *origin=CapeTown&destination=Johannesburg&sensor=false&alternatives=true*

-  #### Headers

    Arguments and data are commonly transferred using the headers of a
    call. You can add data to the headers if the web service requires
    this.

- #### Body{#properties-body}

    The payload of your web service call in the format specified by the
    [Body format](#properties-bodyFormat) property. If you pass data in
    the body, you cannot use the GET [method](#properties-method), but
    need to use POST instead.

- #### Body format{#properties-bodyFormat}

    The [Body](#properties-body) of a request needs to be in the format
    that the web service understands. If you are not sure which value to
    use, the standard and most likely value is 'Text'. The developers of
    the service you are trying to call should be able to assist in
    identifying the correct value.

- #### List of values

    Indicates whether the response should be interpreted as a list of
    values. If this option is selected, you will need to use JSON or XML
    for the [Body format](#properties-bodyFormat).

- #### Output type

    The value type to use when interpreting the response. If the List of
    values option is selected, this is the type to use for each element
    of the list.

    If you create a [custom type](~/Support/BuiltIn/Types/CustomType/) and you have
    formatted your response accordingly, you can point the Output type
    field at your user defined type. After the service has executed,
    Linx will map the return result to the specified structure. Any
    field that is specified in the return structure that is not present
    in the response will be ignored.

- #### Proxy name

    The IP address or URL of your proxy server.

- #### Port

    The web service call is commonly performed over port 80, but you can
    change that if you have configured the service or proxy to use a
    different port.

- #### Bypass on local

    While you are developing the function you may have a different setup
    from the live environment. When this property is checked, the proxy
    setup is ignored for your local machine.

Links
-----

[Wikipedia: Representation state transfer (REST)](http://en.wikipedia.org/wiki/Representational_state_transfer)

[Code Project: Everything About REST Web Services - What and How](http://www.codeproject.com/Articles/21174/Everything-About-REST-Web-Services-What-and-How-Pa)

[IBM developerWorks: RESTful Web services - The basics](http://www.ibm.com/developerworks/webservices/library/ws-restful/)
