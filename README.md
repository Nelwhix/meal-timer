
# Meal Timer
I have a problem where I am always snacking even though I am not really hungry. So I am building a personal swiftui app to help with that. So far I use the native countdown timer on my iPhone but the ios27 release made it slow and annoying. The way the app works is simple
- User opens the app and it asks how long should a meal timer be set for. My default is 2hrs. Anytime I get the first hunger signal I can usually hold it in for 2 more hours.
- We are also hinging on adaptation, if a user frequently extends the timer after the first 2 hours we increase the timer. if a user always ends the timer before the 2 hour threshold. we make it smaller
- All data is local and does not leave the device.
- We could use logic or local AI model for detecting the user's average count
