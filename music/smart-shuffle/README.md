# Smart Shuffle

Music shuffling has remained the same for a very long time. There are times where you might wish to shuffle "just right"; a shuffle that is just long enough to last you on your drive or walk home, and no longer.

Using geolocation and geofencing, a smart shuffle may be able to determine how long it will take you to reach a certain destination. It will then pick songs that total to a length that is equal to or shorter than your commute.

Ideally, Smart Shuffle will be an option in a settings panel for the current music application. However, it may appear alongside the expected shuffle button in that same music application.

## Concepts

### First Run

- Application asks permission to access the current location. If permission is not granted, the feature will not attempt to continue any further.
- Application asks for the user's home and/or work address. If neither is provided, it will do its best to "learn" the user's home and work addresses.
- Application estimates the commute time based on the user's current speed. 

### Subsequent Runs

- Smart Shuffle is activated through settings or a button.
- The generated shuffle subtracts any songs that exceed the estimated commute time, if there are any.
- Smart Shuffle starts playing the modified shuffle.
