# csvParser_Python
Copy csv file content to a dictionary in python

# Introduction
 Your task is to read the input DATAFILE line by line, and for the first 10 lines (not including the header)
 split each line on "," and then for each line, create a dictionary
 where the key is the header title of the field, and the value is the value of that field in the row.
 The function parse_file should return a list of dictionaries,
 each data line in the file being a single list entry.
 Field names and values should not contain extra whitespace, like spaces or newline characters.
 You can use the Python string method strip() to remove the extra whitespace.
 You have to parse only the first 10 data lines in this exercise,
 so the returned list should have 10 entries!
 
 # Sample Input file content
 Title,Released,Label,UK Chart Position,US Chart Position,BPI Certification,RIAA Certification
Please Please Me,22 March 1963,Parlophone(UK),1,-,Gold,Platinum
With the Beatles,22 November 1963,Parlophone(UK),1,-,Platinum,Gold
Beatlemania! With the Beatles,25 November 1963,Capitol(CAN),-,-,,
Introducing... The Beatles,10 January 1964,Vee-Jay(US),-,2,,
Meet the Beatles!,20 January 1964,Capitol(US),-,1,,5xPlatinum
Twist and Shout,3 February 1964,Capitol(CAN),-,-,,
The Beatles' Second Album,10 April 1964,Capitol(US),-,1,,2xPlatinum
The Beatles' Long Tall Sally,11 May 1964,Capitol(CAN),-,-,,
A Hard Day's Night,26 June 1964,United Artists(US)[C],-,1,,4xPlatinum
,10 July 1964,Parlophone(UK),1,-,Gold,
Something New,20 July 1964,Capitol(US),-,2,,Platinum
Beatles for Sale,4 December 1964,Parlophone(UK),1,-,Gold,Platinum
Beatles '65,15 December 1964,Capitol(US),-,1,,3xPlatinum
Beatles VI,14 June 1965,"Parlophone(NZ), Capitol(US)",-,1,,Platinum
Help!,6 August 1965,Parlophone(UK),1,-,Platinum,
,13 August 1965,Capitol(US)[C],-,1,,3xPlatinum
Rubber Soul,3 December 1965,Parlophone(UK),1,-,Platinum,
,6 December 1965,Capitol(US)[C],-,1,,6xPlatinum
Yesterday and Today,15 June 1966,Capitol(US),-,1,,2xPlatinum
Revolver,5 August 1966,Parlophone(UK),1,-,Platinum,
,8 August 1966,Capitol(US)[C],-,1,,5xPlatinum
Sgt. Pepper's Lonely Hearts Club Band,1 June 1967,"Parlophone(UK), Capitol(US)",1,1,3xPlatinum,11xPlatinum
Magical Mystery Tour,27 November 1967,"Parlophone(UK), Capitol(US)",31[D],1,Platinum,6xPlatinum
The Beatles,22 November 1968,"Apple(UK), Capitol(US)",1,1,Platinum,19xPlatinum
Yellow Submarine,13 January 1969,"Apple(UK), Capitol(US)",3,2,Silver,Platinum
Abbey Road,26 September 1969,"Apple(UK), Capitol(US)",1,1,2xPlatinum,12xPlatinum
Let It Be,8 May 1970,"Apple(UK),United Artists(US)",1,1,Gold,4xPlatinum
 
 # Sample Output 
 ('data:', [{'Title': 'Please Please Me', 'UK Chart Position': '1', 'Label': 'Parlophone(UK)', 'Released': '22 March 1963', 'US Chart Position': '-', 'RIAA Certification': 'Platinum', 'BPI Certification': 'Gold'}, {'Title': 'With the Beatles', 'UK Chart Position': '1', 'Label': 'Parlophone(UK)', 'Released': '22 November 1963', 'US Chart Position': '-', 'RIAA Certification': 'Gold', 'BPI Certification': 'Platinum'}, {'Title': 'Beatlemania! With the Beatles', 'UK Chart Position': '-', 'Label': 'Capitol(CAN)', 'Released': '25 November 1963', 'US Chart Position': '-', 'RIAA Certification': '', 'BPI Certification': ''}, {'Title': 'Introducing... The Beatles', 'UK Chart Position': '-', 'Label': 'Vee-Jay(US)', 'Released': '10 January 1964', 'US Chart Position': '2', 'RIAA Certification': '', 'BPI Certification': ''}, {'Title': 'Meet the Beatles!', 'UK Chart Position': '-', 'Label': 'Capitol(US)', 'Released': '20 January 1964', 'US Chart Position': '1', 'RIAA Certification': '5xPlatinum', 'BPI Certification': ''}, {'Title': 'Twist and Shout', 'UK Chart Position': '-', 'Label': 'Capitol(CAN)', 'Released': '3 February 1964', 'US Chart Position': '-', 'RIAA Certification': '', 'BPI Certification': ''}, {'Title': "The Beatles' Second Album", 'UK Chart Position': '-', 'Label': 'Capitol(US)', 'Released': '10 April 1964', 'US Chart Position': '1', 'RIAA Certification': '2xPlatinum', 'BPI Certification': ''}, {'Title': "The Beatles' Long Tall Sally", 'UK Chart Position': '-', 'Label': 'Capitol(CAN)', 'Released': '11 May 1964', 'US Chart Position': '-', 'RIAA Certification': '', 'BPI Certification': ''}, {'Title': "A Hard Day's Night", 'UK Chart Position': '-', 'Label': 'United Artists(US)[C]', 'Released': '26 June 1964', 'US Chart Position': '1', 'RIAA Certification': '4xPlatinum', 'BPI Certification': ''}, {'Title': '', 'UK Chart Position': '1', 'Label': 'Parlophone(UK)', 'Released': '10 July 1964', 'US Chart Position': '-', 'RIAA Certification': '', 'BPI Certification': 'Gold'}])
