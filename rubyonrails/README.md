EasyCode - Ruby On Rails Version
=

EasyCode is a simple webpage that is designed to highlight the ease with which changes can be pushed to production using Cloud Foundry. 
The page will display a greeting as well as a Google map of the location specified in `@location` variable in the `app/controllers/main_controller.rb` file. The code 
will accept any location that Google Maps accepts, such as:

*	City and State. e.g. "Philadelphia, PA"
*	Airport codes. e.g. "BOS"
*	Addresses. e.g. "176 South Street Hopkinton, MA 01748"
*	Landmarks. e.g. "Grand Canyon"


To Push to Cloud Foundry:
-
* Edit the Cloud Foundry `manifest.yml` file and change the `name` parameter to something unique
* `cf push` to send to Cloud Foundry

To Update:
-
* Edit the `@location` variable in the `app/controllers/main_controller.rb` file 
* `cf push` to send the updated code to Cloud Foundry