Hi all, 
I am basically a student and I am working on a very new project i.e to Display a CSV file in line protocol format, that can be used as input to influxdb ?


so help me out to complete my project with ur valuable suggestions and corrections of my mistakes...!!! :)


How do I display a CSV file in line protocol format, like influxdb uses?

measurement[,tag_key1=tag_value1...] field_key=field_value[,field_key2=field_value2] [timestamp]

I am able to read the entire csv file line by line by using the code: with open('test.csv') as fp: for line in fp: print line and i'm getting the o/p as :

['Date','Time','place','status','action'] ['2 sep 2016','12:05:50:274','abc','on','batery on']['16 sep 2016','12:05:51:275','mbc', 'on','batery on']['22 sep 2016','12:05:52:276','kabc','on','batery on']

Whereas I want the out put to in lineprotocol format/syntax such as: ,tag_key=tag value,field key = field value,timestamp

where, tag_key=tag value should have all string type values from the csv file. value,field key = field value should have all integer type values from the csv file.

And timestamp should contain the converted epoch value of date column in the csv file.
