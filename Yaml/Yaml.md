Yaml is a data serialization language that is used for writing configuration files. It is human readable and it is easy to understand.

Uses python indentation to indicate nesting
Tab is not used, thus Space is used to specify indentation.  

The structure of a YAML file is actually a map or a list.
Uses a key and values pairs e.g.

**key**: value
**Name**: "Name"
**Name_list**: ['Name1', 'Name2', 'Name3']


#### Values Type 
YAML can use any scalar values -> null, strings, dates, numbers (ints, floats), bools, list,  and dicts

#### Lists
A list can be defined with a **-**. e.g

List_name:
&nbsp;&nbsp;&nbsp;&nbsp;**-** key1: "Value1"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;key2: "Value2"
&nbsp;&nbsp;&nbsp;&nbsp;**-** key1: "Value3"
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;key2: "Value4"

or using **[]**
List_name: ["Value1", "Value2", "Value3"]


#### Commenting 
You can comment using **#**.

#### Dates
Date format is year-month-day
e.g. **release_date: 2024-05-17**


#### Best practices
The key is are written in Lower case.