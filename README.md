Task 1

File Microsof Access database.accdb

Task 2

There is a bug in 'unsigned int' because it will work even in case of  - value. In this case I consider 'nothrow' wrong because if it doesn't take a new memory it will still go on working. It must either be deleted or we must check the presence of data. The data in 'destructor' must be checked with 'nullptr' as in c++ it is wrong to check the 'pointer' with 'null'. The compiler doesn't give error, but there's a great difference between them. In Set function 'unsigned' must be removed as well, and the exceptions must be presented more clearly. 'Unsigned' must also be removed from Get, and the space between 0 to m_nsize must be checked. Besides, it is necessary to form 'exception' in 'else' correctly because even if it takes a value greater than 'size', it won't give an error anyway and will bring back the default value of 0. 
If we deal with Array we must remove Set function because Array is a static STL and it must get all the values through the constructor.
