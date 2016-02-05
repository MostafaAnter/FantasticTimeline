# FantasticTimeline
customized list view like Facebook, Google+ news feed where it contains multiple images and texts.

# steps
- Create a new project in Eclipse from File ⇒ New ⇒ Android Application Project and fill all the required information.
- Open res ⇒ values ⇒ dimens.xml and add dimens
- Open res ⇒ values ⇒ colors.xml and add colors
- Under res ⇒ drawable, create a new file called bg_parent_rounded_corner.xml 
- To keep the project well organized, I am creating required packages first. Create 4 packages named app, adapter, data and volley. 
- Create a class named LruBitmapCache.java under volley package and add the following code. This class takes care of caching network images on disk.
