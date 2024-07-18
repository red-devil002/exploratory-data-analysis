# Handle Invalid Values
1. Encode Unicode properly
* In case the data is being read as
junk characters, try to change
encoding, E.g. CP1252 instead of
UTF-8

2. Convert incorrect data types
* Correct the incorrect data types
to the correct data types for ease
of analysis. E.g. if numeric values
are stored as strings, it would not
be possible to calculate metrics
such as mean, median, etc.

* Some of the common data type
corrections are — string to
number: "12,300" to “12300”; string
to date: "2013-Aug" to “2013/08”;
number to string: “PIN Code
110001” to "110001"; etc

3. Correct values that go
beyond range 
* If some of the values are beyond
logical range, e.g. temperature
less than -273° C (0° K), you
would need to correct them as
required.

* A close look would help you
check if there is scope for
correction, or if the value needs
to be removed.

4. Correct wrong structure
* Values that don’t follow a defined
structure can be removed.

* E.g. In a data set containing pin
codes of Indian cities, a pin code
of 12 digits would be an invalid
value and needs to be removed.
Similarly, a phone number of 12
digits would be an invalid value