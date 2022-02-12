# SignReleaseWithLocalProperties
This is a companion repository for [my blog post on easily signing local Android release builds with `local.properties`](http://mcomella.xyz/blog/2022/autosign-release-builds-android.html).

## Try it out
Add the following to your `local.properties` file:
```gradle
autosignReleaseWithDebugKey=true
```

After syncing your project in Android Studio, you can select "Release" from the "Build Variants" tab and click "Run" to install and run the release build as you would a debug build. You can also install the release variant via the command line: `./gradlew installRelease`. See the blog post for details on how to configure this in your own app.
