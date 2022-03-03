# Data

"NYC SQUIRREL DATABASE"

nyc_squirrels <- readr::read_csv("https://raw.githubusercontent.com/rfordatascience/tidytuesday/master/data/2019/2019-10-29/nyc_squirrels.csv")

## Codebook

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
- `location`: Value is either "Ground Plane" or "Above Ground." Sighters were instructed to indicate the location of where the squirrel was when first sighted.
- `above_ground_sighter_measurement`: For squirrel sightings on the ground plane, fields were populated with a value of “FALSE.”
- `specific_location`: Sighters occasionally added commentary on the squirrel location. These notes are provided here.
- `running`: Squirrel was seen running.
- `chasing`: Squirrel was seen chasing.
- `climbing`: Squirrel was seen climbing.
- `eating`: Squirrel was seen eating.
- `foraging`: Squirrel was seen foraging.
- `other_activities`: other activities
- `kuks`: Squirrel was heard kukking, a chirpy vocal communication used for a variety of reasons.
- `quaas`: Squirrel was heard quaaing, an elongated vocal communication which can indicate the presence of a ground predator such as a dog.
- `moans`: Squirrel was heard moaning, a high-pitched vocal communication which can indicate the presence of an air predator such as a hawk.
- `tail_flags`: Squirrel was seen flagging its tail. Flagging is a whipping motion used to exaggerate squirrel's size and confuse rivals or predators. Looks as if the squirrel is scribbling with tail into the air.
- `tail_twitches`: Squirrel was seen flagging its tail. Flagging is a whipping motion used to exaggerate squirrel's size and confuse rivals or predators. Looks as if the squirrel is scribbling with tail into the air.
- `approaches`: Squirrel was seen approaching human, seeking food.
- `indifferent`: Squirrel was indifferent to human presence.
- `runs_from`: .Squirrel was seen running from humans, seeing them as a threat.
- `other_interactions`: Sighter notes on other types of interactions between squirrels and humans.
- `lat_long`: Combined lat long
- `community_districts`: zip codes
- `borough_boundaries`: Borough boundaries
- `city_council_districts`: City council districts
- `police_precincts`: Police precincts

