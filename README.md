MyGuide Library provides necessary information about the desired city or selected organization and allow users to access personal services of the organization.
 
 Usage:
 Get library package "myguide-library.aar" and place it into the lib folder of your Android Studio project
 
 Add implementation(name:'myguide-library', ext:'aar') into the dependencies section of build.gradle in your module
 
 dependencies {
 
	...
	
    implementation(name:'myguide-library', ext:'aar')
    
	...
	
 }
 
 Get the APIkey to get all the benefits from the library usage. (Visit myguide.city for mor information about APIkey) 
 
 Set the APIkey in your application:

   MyGuide.setAPIKey(<YourAPIKey>);

Show information to user:

	MyGuide.start(Context context);
	
	Available methods:
	
	MyGuide.setAPIKey(<YourAPIKey>); -sets the APIkey for MyGuide Library. should be called  before using start... metods to take effect.
	
	MyGuide.start(Context context); - shows country and city selection UI user can select from the wide range of avaliable cities.
	MyGuide.start(Context context, "Title"); - shows country and city selection UI with the customizable title on top.
	
<img src="https://user-images.githubusercontent.com/91147646/134476464-7ba509e7-6f18-420b-9bc7-79bf04c1b887.png" width="400">  <img src="https://user-images.githubusercontent.com/91147646/134476930-d5ed6493-6572-4abf-8f25-8ce84aaf64b7.png" width="400">	


	MyGuide.startCity(Context context,"<avaliableCityId>"); - shows the selected city information.
	MyGuide.startCity(Context context,"<avaliableCityId>", "Lucerne"); - shows the selected city information with the customizable title on top.
<img src="https://user-images.githubusercontent.com/91147646/134477195-67350325-d202-493b-bb9a-b5a309c8c3e5.png" width="400">

	MyGuide.startPartner(Context context,"<avaliablePartnerId>"); - shows the selected partner information.
<img src="https://user-images.githubusercontent.com/91147646/134477286-ba760d58-aea5-4110-afd7-08fa9c312550.png" width="400">
	MyGuide.startPartner(Context context,"<avaliablePartnerId>", "Title"); - shows the selected partner information with the customizable title on top.
List of avaliable city and partner ids can be found at myguide.city.
