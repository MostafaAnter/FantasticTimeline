# FantasticTimeline
customized list view like Facebook, Google+ news feed where it contains multiple images and texts.

# steps
- Create a new project in Eclipse from File ⇒ New ⇒ Android Application Project and fill all the required information.
- Open res ⇒ values ⇒ dimens.xml and add dimens
- Open res ⇒ values ⇒ colors.xml and add colors
- Under res ⇒ drawable, create a new file called bg_parent_rounded_corner.xml 
- To keep the project well organized, I am creating required packages first. Create 4 packages named app, adapter, data and volley. 
- Create a class named LruBitmapCache.java under volley package and add the following code. This class takes care of caching network images on disk.
- Under app package create class named AppController.java and paste the following content. This is a singleton class which initializes global instances of required classes. All the objects related to volley are initialized here.
- Now open your AndroidManifest.xml file and add Application.java class in <application> tag. Also we need to add INTERNET permission as this app makes network calls.
- The main challenge in this project is adjusting the aspect ratio of feed image once it is downloaded. Unfortunately volley doesn’t provide any callback method once the NetworkImageView is loaded. So I created a custom ImageView class with callback methods. This class automatically adjusts the image height to prevent image aspect ratio distortion.
- التحدى الوحيد ف المشروع هو ضبط ارتفاع الصوره ليتناسب مع عرضها لان الصوره عرضها هيتغير مع اختلاف الجهاز وبالتالى الصوره هتتشوه
- 
