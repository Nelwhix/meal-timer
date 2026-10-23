# Meal Timer

A small, private iOS app that helps you tell real hunger apart from the urge to snack.

## Why

I snack often when I'm not actually hungry. I've noticed that after the first hunger signal I can usually hold off for about two more hours. Until now I used the built-in iOS countdown timer for this, but since iOS 27 it has become slow and awkward. Meal Timer is a dedicated SwiftUI replacement built around that one habit.

## How it works

1. **Start at the first hunger signal.** Open the app and start a meal timer. The default is **2 hours**, and you can pick a different length.
2. **Reach the target or extend it.** When the timer finishes you can eat, or extend by another round of the same length (for example, another 2 hours) if you're still fine.
3. **See how long you held out.** When a session ends, the app shows the total time from start to finish across all rounds, e.g. *"You can clearly hold it off for 2h 30m."*
4. **Ending early counts too.** Stopping before the target means you gave in and ate early. That's recorded so the app can adapt.

### Adaptive timer length

Once a week, Meal Timer looks at your recent sessions and adjusts the default length:

- **Frequent extensions:** the default gets longer.
- **Frequently giving in early:** the default gets shorter.

Whether this uses simple rules or an on-device model is still open.

### Live Activity

The running timer is planned to show as a Live Activity on the Lock Screen and in the Dynamic Island, so you can check it without opening the app.

## Privacy

All data stays on your device. There's no account and no cloud sync, and nothing is sent over the network.

## Requirements

- iOS 27.0 or later
- Xcode with Swift 5 language mode

## Getting started

```sh
git clone https://github.com/Nelwhix/meal-timer.git
cd meal-timer
open meal-timer.xcodeproj
```

Then pick an iPhone simulator or device and run the app.

## Status

This is an early-stage personal side project. The repository currently contains the Xcode project scaffold, and the features above are being built step by step.
