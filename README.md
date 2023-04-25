# Html Table Writer Program.

## This is simple program to convert your python data tables into html tables.

### Guidelines to use this program:

1. import the program.

2. create a table object.

3. write a table using write_table function. 

4. To add more rows after you wrote it for first time, use extend_table function.

### Sample code:
    import html_table_writer
    html_table = html_table_writer.table(file)
    html_table.write_table(data)
    html_table.extend_table(data)

Note: the data used while writing or extend the table should be of the following form
[[row itmes],[row items],....] where rows should be tuples or lists.

## Stlying your html table:

### Use the following style options while first creating the table.

• headers: all the headers of your table in order of how your row data is stored. this should be tuple or a list.

• encoding: the encoding of the data.

• align: alignment of the table on the page. (left/right/center)

• bg_color: background color of your table.

• text_color: color of the text of your table.

• border (int): the width of border if needed.

• border_color: the color of border of the table.

#### Below is an example of code with stylish table:

    html_table = html_table_writer.table('table.html',headers=['sr no.','name'],encoding='utf-8',align='left',bg_color='white',text_color='black',border=2,border_color='black',)

    html_table.write_table([(1,'arjun'),(2,'soumya'),(3,'ali')])

#### Here's the output of above code:
![Output code.](https://i.ibb.co/zZzDbDS/output-demo.png)
