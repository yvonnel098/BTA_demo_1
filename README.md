BTA_demo_1
==========

Android App for the Open Bible Translation creation story layouts.  This application includes three main activities
1. Splash screen
  - implemented by:  SplashActivity.java with res/anim/fade-in.xml and res/layout/activity_splash.xml
2. A navigational list view
  - implemented by: 
    - MenuListActivity.java with res/layout/activity_menu_list.xml
    - MenuListFragment.java, rowAdapter.java with res/layout/menu_list, menu_item.xml
3. Translation Detail screen  
  - implemented by:  
    - TranslationDetailActivity.java with res/layout/activity_translation_detail.xml
    - TranslationFragment with res/layout/fragment_translation.xml

The dummy section contains holder text for a list view.  It is currently not being used.

The calling sequence is as follows:
Splash screen->Navigational List View->Translation Detail Screen.

At this point, all resources are hard coded and I only implemented one horizontal landscape.  Neither fragments
activities have saved states.

I used Android Studio version 0.5.4.  The project is compiled using Gradle.  Although the project is currently compiled with
min SDK level of 11 and target SDK level of 19, I started off with min SDK level of 8.  As a result, MenuListFragment.java 
is using the support library to address fragments.  I was having problem with the SDK manager not loading sdk level 11.  
This should clear up with feature iterations.
