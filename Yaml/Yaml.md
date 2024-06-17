Yaml is a data serialization language that is used for writing configuration files. It is human readable and it is easy to understand.

Uses python indentation to indicate nesting
Tab is not used, thus Space is used to specify indentation.  

The structure of a YAML file is actually a map or a list.
Uses a key and values pairs e.g.

**Key**: value
**Name**: "Name"
**Name_list**: ['Name1', 'Name2', 'Name3']


Values 
YAML can use any scalar values -> null, strings, dates, numbers (ints, floats), bools, list,  and dicts

A list of keys can be defined with a **-**. e.g

List_name:
&nbsp;&nbsp;&nbsp;&nbsp;**-** Key1: "Value1"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Key2: "Value2"
&nbsp;&nbsp;&nbsp;&nbsp;**-** Key1: "Value3"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Key2: "Value4"
