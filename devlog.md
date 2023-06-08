---
title: AED Sim Developer Log
---

These are my unedited notes I've kept while creating the latest version of AED Sim. They contain spelling mistakes and grammar errors. I'm posting them to help give people an idea of what goes into to building apps as the process for non-developers is quite opaque.

Jun 8

- [x] 3.0.0 version released 🥰🎉 (need to fix some typos in the App Store description 🤦‍♂️)
- [x] Website updated

Jun 7

- [x] Update app website screenshots
- [x] Create raw footage for demo movie
- [x] Edit demo movie
- [x] Update app description
- [x] Add all info to App Store
- [x] Submit for release
- [x] Fixed accessibility issues I noticed with Voice Over.

Jun 6

- [x] Renamed to AED Sim because an app no longer for sale on the App Store is squatting on AED Simulator. Figured since I’m using aedsim.com for the domain might as well rename the project as that. Hopefully SEO built up carries forward.
- [x] Fixed issues with languages and initial launch so that US English users get US English and Commonwealth English users get UK English. Seems a bit silly to sweat about this stuff but I only speak English so doing everything I can to get the app ready for localization with languages I can read.
- [x] WWDC is on this week and all the amazing tech is distracting from actually getting AED Sim from launching.

Jun 5

- [x] Localize all strings, remove all unused strings
- [x] Remove all but en and en-GB languages
- [x] Submit test flight build
- [x] Considered associating .aedsim files with app so that they can be shared and then opened but decided this is getting too complicated.
- [x] Investigate Cloud Kit for documents support but decided against it as I was going down a rabbit hole I didn't need to go at this time.

Jun 4

- [x] Vibrate on shock (even when device in silent mode)
- [x] Don’t loop on pushAnalyze or pushShock if interval is zero
- [x] Profiles are saved and restored from Profiles directory
- [x] Improved support for multiple profiles without adding complexity if only one is used (which will likely be the majority of all users)
- [x] Profile has a languageCode “en”

Jun 3

- [x] Fix app icon color profile. Seems like Pixelmalator assigned something other than sRGB which made it duller and different than the current version. Using the sRGB profile fixed this.
- [x] Added support for iOS 15 and above. Was previously targeting 16+ but realized I wasn’t using much that was introduced in 16. Investigated supporting iOS 14 but a lot more significant changes would be needed. But the % of devices still on that OS doesn’t make sense. 1-5% depending on where you look.
- [x] Remove sheet close buttons on all views except the root Settings View. Since the built in views from pickers don’t allow for them it started to feel completely random why some screen had this shortcut and others didn’t. Until I get a definitive answer on when to include them I’ll keep it off. When in doubt, leave it out.
- [x] Improve layout on smaller devices like my trusty old iPhone SE (1st edition)
- [x] Allow optional speech on state state. Default prompts don’t speak at this state but some devices might want to put some initial instructions, like, “Ensure 911 has been notified”.

Jun 2

- [x] Initial test flight build submitted and approved.

Jun 1

- [x] Add button to open app documents folder
- [x] Make AED state strings accessible from any language so that English speaking users will be able to operate the AED in another language.
- [x] Load other languages into current profile
- [x] Allow selecting any voice
- [x] Remove cloth background, doesn’t make sense

May 30

- [x] Rename Start state name
- [x] Improve Settings button
- [x] Improve layout for dynamic type at accessibility sizes
- [x] Improve mode names
- [x] Correctly hide status bar
- [x] Decide that “en” shall be US English since it’s the biggest marker for apps and the version of English I use while programming.
- [x] Localize all strings in the app (good comments are still needed)
- [x] Localize en-GB strings
- [x] Auto translated Japanese, Chinese, and Hebrew (RTL) for testing. Results were great.

May 28 - 29

- [x] Use MP4 Apple Lossless for all audio files
- [x] Display doesn’t animate when turning on/off
- [x] Play sound effects correctly
- [x] Move all logic back to code and delete unneeded files
- [x] Fix metronome not playing
- [x] Add ability to loop sounds
- [x] Fix sound not playing when in silent mode
- [x] Advanced settings editor
- [x] Custom sound effects picker
- [x] Save advanced settings in user defaults
- [x] Add Close/Done buttons to all sheets
- [x] Custom background images picker

May 27

- [x] Noticed that aedsim.com was available so I snagged it and setup the site on CloudFlare pages.
- [x] Updated gshaw.ca to point to aedsim.com. https://favicon.io is wonderful

May 2023

AED Sim started way back in 2010 when I was working as paramedic for BC Ambulance Service and volunteering as a fire fighter.

I was frustrated when teaching CPR to other members of the fire department about the lack of AED trainers because of their costs. These devices look like AEDs but are essentially toys yet they cost hudreds of dollars.

At this time I jsut received an iPhone 3GS and realized I could create simulator on the phone that would get most of the benefit of training without almost none of the cost.

The app launched as iDefibrillate using the trendy at the time "i" prefix. The name hasn't aged well so when it was time to do a much needed update I've renamed the app as the more practical AED Sim.

Sometime in 2010

- [x] Intial version released on the App Store!
