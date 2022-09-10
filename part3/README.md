# Programming Skill Assessment for Research Assistants
## Mind in Society Lab
**Deadline:** ***Wednesday, September 14, 2022, by 11:59 PM ET***.

Assessment for `TODO: name` (`TODO: email`)

**Please make sure you read ALL instructions and complete ALL parts asked of you.**

---
## Instruction
### Part 3: Working with the Google Street View API
We also utilize the Google Street View API very frequently for our projects. To complete this part, review the [documentations for the Static SV API](https://developers.google.com/maps/documentation/streetview/overview).

You will also need the `keys.json` file you've loaded in part 1.

#### Task 1: Load the API key file
Load the `keys.json` file into the jupyter notebook, and assigned it to the `keys` variable. Then, access the actual key inside and assigned it to the `API_Key` variable.

#### Task 2: Complete the API request query URL
Review the [query documentation](https://developers.google.com/maps/documentation/streetview/request-streetview) and complete the request URL using an f-string inside the `get_SV_images` function. Utilize both static values and variables as parameters in your query string. 

Follow the specifications below:
- The output size of each image should be 640px by 400px
- The locations should be the coordinates specified by the function parameters
- The search radius should be 250 meters
- Use the specified angles to adjust the heading of the camera
- Make sure to only use outdoor images
- Lastly, use the `API_Key` for your request, no signature needed

#### Task 3: Test your query
Test your `get_SV_images` function by using the following coordinates:

- Location 1: `(37.808967, -122.473655)` - you should see a location near the Golden Gate Bridge.
- Location 2: `(37.871907, -122.258287)` - you should see a location on the UC Berkeley campus.
- Location 3: `(42.276582, -83.735750)` - you should get a location by Weiser Hall on the UM campus.

--
### Make sure to commit your changes often! 
To submit, you should have a completed `get_SV_images` function, along with the output images for the 3 locations inside of your jupyter notebook. 