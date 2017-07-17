AddToList
=========

The AddToList function allows lists to be populated. Use this function
when you want to populate a list with some data.

In order to add items to a list you need ... a list. Go to
[Types](~/Support/BuiltIn/Types/) and select a [List](~/Support/BuiltIn/Types/List/) or create your own
[custom type](~/Support/BuiltIn/Types/CustomType/). Then drag the List into your process
and populate it with data.

Properties
----------

-  #### List

    The list to populate. If you don't have this list in your drop-down
    as yet, add a 'Type' -\> 'List' into your process before this
    function in the process sequence. If you need a multi-column list,
    you need to add a 'custom type' that defines the columns you need
    and select the type when you create your list. That list object will
    then appear in the drop-down for this function for you to select.

-  #### Value

    The values you want to add to the list. The columns in this list
    were defined in the 'Type' -\> 'List' function mentioned above. When
    you point this function to a list, the columns from that list will
    appear in the 'Value' property window. You can point a database
    query or any other data source to this property that returns the
    data with all specified columns for that user defined type.

List Output
-----------

You can point the value field of the AddToList function at a SQLExecute
function output as long as you switch off 'Loop Results' in the
SQLExecute function properties. When 'Loop Results' is off the query
will return a list.

Other functions also output lists, including the File List function.
