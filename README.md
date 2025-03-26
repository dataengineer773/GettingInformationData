We want to view some characteristics of a DataFrame, One of the easiest things we can do after loading the data is view the first few rows using head, We can also take a look at the number of rows and columns,
We can get descriptive statistics for any numeric columns using describe, After we load some data, it is a good idea to understand how it is structured and what kind of
information it contains. Ideally, we would view the full data directly. But with most real-world cases,
the data could have thousands to hundreds of thousands to millions of rows and columns. Instead, we
have to rely on pulling samples to view small slices and calculating summary statistics of the data.
In our solution, we are using a toy dataset of the passengers of the Titanic on her last voyage. Using
head we can take a look at the first few rows (five by default) of the data. Alternatively, we can use
tail to view the last few rows. With shape we can see how many rows and columns our DataFrame
contains. And finally, with describe we can see some basic descriptive statistics for any numerical
column.
It is worth noting that summary statistics do not always tell the full story. For example, pandas treats the
columns Survived and SexCode as numeric columns because they contain 1s and 0s. However, in this
case the numerical values represent categories. For example, if Survived equals 1, it indicates that the
passenger survived the disaster. For this reason, some of the summary statistics provided don’t make
sense, such as the standard deviation of the SexCode column (an indicator of the passenger’s gender).
