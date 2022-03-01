# data

nyc_squirrels <- readr::read_csv("https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2019/2019-10-29/nyc_squirrels.csv")

## name of data file

- `long`: Longitude
- `lat`: Latitude
- `unique_squirrel_id`: Identification tag for each squirrel sightings. The tag is comprised of "Hectare ID" + "Shift" + "Date" + "Hectare Squirrel Number."
- `hectare`: ID tag, which is derived from the hectare grid used to divide and count the park area. One axis that runs predominantly north-to-south is numerical (1-42), and the axis that runs predominantly east-to-west is roman characters (A-I).
- `shift`: Value is either "AM" or "PM," to communicate whether or not the sighting session occurred in the morning or late afternoon.
- `date`: Concatenation of the sighting session day and month.
- `hectare_squirrel_number`: Number within the chronological sequence of squirrel sightings for a discrete sighting session.
- `age`: Value is either "Adult" or "Juvenile."
- `primary_fur_color`: Value is either "Gray," "Cinnamon" or "Black."
- `highlight_fur_color`: Discrete value or string values comprised of "Gray," "Cinnamon" or "Black."
- `combination_of_primary_and_highlight_color`: A combination of the previous two columns; this column gives the total permutations of primary and highlight colors observed.
- `color_notes`: Sighters occasionally added commentary on the squirrel fur conditions. These notes are provided here.
- ...
