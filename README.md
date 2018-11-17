A quick way to enable google maps in a new application:

Get a google maps key for android:

Go to google console
https://console.cloud.google.com

1. create a new project
2. In the project, go to "Enable APIs and get credentials like keys"
3. go to: "+ ENABLE APIS AND SERVICES"
4. enable MAPS SDK for Android
5. In APIs & Services, go to Credentials
6. Create credentials
7. hit API key
8. copy the key



in AndroidManifest.xml paste in the key:
<meta-data
            android:name="com.google.android.geo.API_KEY"
            android:value="sdoifjewkfjdsikfoiuwefkljhsdfoi" />


To get the layout visible in Design tool. Make sure to add "Base" in styles.xml
<style name="AppTheme" parent="Base.Theme.AppCompat.Light.DarkActionBar">

in build.gradle add:
implementation 'com.google.android.gms:play-services-maps:15.0.1'


Create a new activity class for the maps, also add this activity class in AndroidManifest.xml
<activity
            android:name=".MapsActivity"
            android:parentActivityName="MainActivity">
</activity>

