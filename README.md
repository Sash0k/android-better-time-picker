## About


TimePicker DialogFragment modeled after the 4.2 Alarm Clock TimePicker to improve UX for picking time


## Changelog:

**1.1**
  
  * Fix for the bold text overflow on Android 4.3 and 4.4
  * Updated the compatibility library to the latest one at the moment

**1.0**
  
  * Based on the version 1.2.0 of the [BetterPickers][5] project


Including in Your Project


Android better time picker is an [Android library project][7].

You can include this project by [referencing it as a library project][8] in Eclipse or ant.

If you are a Maven user you can easily include the library by specifying it as
a dependency:

    <dependency>
      <groupId>com.doomonafireball.betterpickers</groupId>
      <artifactId>library</artifactId>
      <version>1.2.0</version>
      <type>apklib</type>
    </dependency>

## Dependencies

*You will need these fonts*
    Roboto-Bold.ttf
    AndroidClockMono-Thin.ttf

These can be fount in you android SDK folder or in the `assets/fonts` folder



## Usage


*For a working implementation of this project see the `sample/` folder.*

  0. Include the Android clock fonts in your `assets/fonts/` folder (create the folder if it doesn't already exist.  You can find these fonts in the `assets/fonts/` folder in this library or in your android SDK installation.

        AndroidClockMono-Thin.ttf

  1. Implement the appropriate Handler callbacks:
Implement the `TimePickerDialogHandler` for any class that you want to be notified when the time is set

  2. Use one of the Builder classes to create a PickerDialog with a theme:

        TimeickerBuilder btp = new TimeickerBuilder()
            .setFragmentManager(getSupportFragmentManager())
            .setStyleResId(R.style.BetterPickersDialogFragment);
        btp.addTimeSetListener(this); //add here any listener implementing TimePickerDialogHandler 
        btp.show();


## Theming


Please see the [original better android pickers documentation][5] for theming capabilities



## Contribution


Feel free to contribute to [BetterPickers][5].



## Credits

Thanks to Derek Brameyer for his work on [Android Better Pickers][5].



## License


    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.


 [5]:https://github.com/derekbrameyer/android-betterpickers
 [6]: https://play.google.com/store/apps/details?id=com.doomonafireball.betterpickers.sample
 [7]: http://developer.android.com/guide/developing/projects/projects-eclipse.html
 [8]: http://developer.android.com/guide/developing/projects/projects-eclipse.html#ReferencingLibraryProject
 [9]: http://viewpagerindicator.com/
 [10]: https://github.com/derekbrameyer/android-betterpickers/issues/new
 [11]: https://plus.google.com/108284392618554783657/posts
 [12]: http://willowtreeapps.github.io/OAK/
 [13]: http://www.willowtreeapps.com/
