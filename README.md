# FragmentExampleExtended

* To add a Fragment statically to an Activity so that it is displayed for the entire lifecycle of the Activity, declare the Fragment inside the layout file for the Activity using the <fragment> tag. You can specify layout attributes for the Fragment as if it were a View. 
* To add a Fragment dynamically to an Activity so that the Activity can add, replace, or remove it, specify a ViewGroup inside the layout file for the Activity such as a FrameLayout. 
* When adding a Fragment dynamically to an Activity, the best practice for creating the fragment is to create the instance with a newinstance() method in the Fragment itself. Call the newinstance() method from the Activity to create a new instance.
* To get an instance of FragmentManager, use getSupportFragmentManager() in order to instantiate the Fragment class using the Support Library so your app remains compatible with devices running system versions as low as Android 1.6.
* To start a series of Fragment transactions, call beginTransaction() onaFragmentTransaction. 

With FragmentManager your code can perform the following Fragment transactions while the app runs, using FragmentTransaction methods:
* Add a Fragment using add().
* Remove a Fragment using remove().
* Replace a Fragment with another Fragment using replace().
