MyGuide Library provides necessary information about the desired 
city or selected organization and allow users to access personal
 services of the organization.
 
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

	![country-selection](https://user-images.githubusercontent.com/91147646/134462800-e5c18ee4-9e3a-414d-afbf-64af426513ba.png)

	![city-selection](https://user-images.githubusercontent.com/91147646/134462820-68b9ff9c-ce95-4928-a8bf-35067dffa8ff.png)

	MyGuide.startCity(Context context,"<avaliableCityId>"); - shows the selected city information.
	MyGuide.startCity(Context context,"<avaliableCityId>", "Title"); - shows the selected city information with the customizable title on top.
	
	![city ](https://user-images.githubusercontent.com/91147646/134462326-6cc30ad6-f1e3-4ddc-a5ea-2222081cd458.png)
	
	MyGuide.startPartner(Context context,"<avaliablePartnerId>"); - shows the selected partner information.
	MyGuide.startPartner(Context context,"<avaliablePartnerId>", "Title"); - shows the selected partner information with the customizable title on top.
	
	![partner](https://user-images.githubusercontent.com/91147646/134462859-5287402c-b3fd-4100-9320-80b484dea44f.png)

List of available city and partner ids can be found at myguide.city.
