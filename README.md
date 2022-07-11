# Graphing dino funworld
 Data Visualization Project

Provided Database
The database provided by the park administration is formatted to be readable by any SQL database library. The course staff recommends the sqlite3 library. The database contains three tables, named 'checkins', 'attractions', and 'sequences'. The information contained in each of these tables is listed below:

checkins:

- Description: check-in data for all visitors for the day in the park. The data includes two types of check-ins, inferred and actual checkins.

- Fields: visitorID, timestamp, attraction, duration, type

 

attraction:

- The attractions in the park by their corresponding AttractionID, Name, Region, Category, and type. Regions are from the VAST Challenge map such as Coaster Alley, Tundra Land, etc. Categories include Thrill rides, Kiddie Rides, etc. Type is broken into Outdoor Coaster, Other Ride, Carussel, etc.

- Fields: AttractionID, Name, Region, Category, type

sequences:

- The check-in sequences of visitors. These sequences list the position of each visitor to the park every five minutes. If the visitor has not entered the part yet, the sequence has a value of 0 for that time interval. If the visitor is in the park, the sequence lists the attraction they have most recently checked in to until they check in to a new one or leave the park.

- Fields: visitorID, sequence

The database file is named 'dinofunworld.db' and is available in the readonly directory of the Jupyter Notebook environment (i.e. readonly/dinofunworld.db).

Assignment
The administrators would like you to create four graphs: a pie chart, a bar chart, a line chart, and a box-and-whisker plot. All of these plots can be created with the data provided.

Chart 1: A Pie Chart depicting visits to thrill ride attractions.

Chart 2: A Bar Chart depicting total visits to food stalls.

Chart 3: A Line Chart depicting attendance at the newest ride, Atmosfear over the course of the day.

Chart 4: A Box-and-Whisker Plot depicting total visits to the park's Kiddie Rides.
