# An Introduction to React Native for Web Devs

## Taking your first steps in mobile development

If you're familiar with HTML, CSS, Javascript - maybe you've even dabbled in a bit of React or other declarative JS frameworks - and you're suddenly facing the prospect of working on a mobile app, then this article is for you!

First things first, what is mobile development? How is it different from standard web development for mobile devices? 

### Mobile Operating Systems

Let's talk a little about operating systems. An operating system is:

> ...system software that manages computer hardware, software resources, and provides common services for computer programs.

The most common operating systems on personal computers are Microsoft Windows (at 77% of PCs), Apple's MacOS (18%), and Linux (various flavours, 2%). 

![operating systems](https://cdn.hashnode.com/res/hashnode/image/upload/v1646828895956/85e_X0XmR.png)

There are basically just two players on the scene providing operating systems for mobile devices: Google and Apple. 72% of mobiles run Google's Android OS, and 12% run iOS, which is Apple's operating system for mobiles. 

*Note that the mobile operating systems are not just used on mobiles. They are used in tablets, wearables like smart watches, smart TVs...etc.*

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646829114459/TFydZ7iIK.png)

iOS is mostly written in Objective-C and Swift, while Android is mostly written in Java and Kotlin. 

With two very common OSs among mobile devices, historically this has meant that anyone wanting to make an app has either had to pick an operating system to write their app for (e.g. an Android-only app), or create and maintain two separate codebases (one for each OS). 

### Writing Cross-Platform Software

Writing cross-platform software means writing software that can run on more than one operating system with the same code. Given the thousands of reasons why this is advantageous, it's no surprise that this is considered to be the holy grail of software development!

![a grail](https://cdn.hashnode.com/res/hashnode/image/upload/v1646829449854/QWMQKN0R7.png)

Some of the reasons why tech companies love cross-platform software:

- ONE codebase
- ONE development team
- Consistency across operating systems
- Easier to maintain
- Usually quicker to develop
- Easier to roll out changes/bug fixes
- Cheaper (fewer devs required, less specialised software/hardware)
- Can reach a wider audience (by catering to more operating systems)
- Reusable code
- ... and many more reasons!

### Enter: React Native

This is where React Native steps in!

![react native](https://cdn.hashnode.com/res/hashnode/image/upload/v1646829652240/uHacFIVY8.png)

React Native was basically invented to solve the problem of writing mobile apps for different operating systems. 

If you look at the [React Native website](https://reactnative.dev/), these phrases form its elevator pitch:

- "Learn once, write anywhere"
- "Create native apps for Android and iOS using React"
- "Written in Javascript, but rendered with native code"

### What is "Native" anyway?

When I first started learning React Native, I realised I didn't really know what the "Native" part meant.

Here's the dictionary definition:

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646829935027/hJYosOhP3.png)

1. Being the place or environment in which a thing came into being.

2. Belonging to a thing by nature; inherent

In the context of software, this means that "native software" is software that runs directly on the device, in the environment of the device's full operating system, interacting and interfacing with the device's OS code.

You can contrast a native app, which is downloaded and installed on the device (e.g. through the Google Play Store or the Apple Store) with a web app, which does not require installation. 

A web app's software runs on a **browser** and can only operate in the environment provided by the browser. 

(A browser is itself a native app). 

Take a look at the image below to see the differences between a web app and a native app:

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646830208846/NfbwXBw9J.png)

In this example of Yelp's restaurant search, the web app is basically the same website you'd view on a PC, but condensed down to a mobile sized screen. You can see that the red toolbar is framed by the browser toolbar - the software is running inside the browser app. 

Contrast this with the image of the mobile app on the left, and you can see that there is no browser framing the screen - the red extends all the way up, even into the mobile's status bar. It is interacting directly with the code that displays the status bar because it can interface directly with the operating system's code. 

Note also that the mobile app benefits from being able to access a few mobile-specific features. For example, in the toolbar at the bottom of the screen, you can see a "Nearby" button that is likely to use the device's geolocation functionality to bring up restaurants near the user. 

### How does React Native help?

React Native allows you to use Javascript to access the device's native features. It essentially acts as a "bridge", or a translation service, between the device's native code, and Javascript.

![bridge](https://cdn.hashnode.com/res/hashnode/image/upload/v1646830568795/1lsxwVOl6.png)

This means that as well as being able to create apps for multiple platforms using the same codebase, apps written in React Native are *natively rendered* which is good for performance, and the UI (the apps look "natural", like they were made out of OS code all along). 

Here are some other pros of React Native: 

- Very similar to React. If you know React already, you can pretty quickly pick up how to use React Native. 
- Declarative coding
- Component-based
- Refresh app to see changes (no rebuilds)
- Can make use of device's persistent storage (unlike browsers where storage can be unreliable or rely on a cache)
- Improved privacy having data local to the device
- Can use your usual code editor (e.g. VSCode) rather than a mobile specific code editor.

### Let's see some code!

Now we have some context on mobile development and React Native, let's look at some code! 


```
import { Text } from 'react-native';
import * as React from 'react';

const HelloWorldApp = () => {  
   return 
      <Text>Hello world!</Text>
}

export default HelloWorldApp;

``` 

So far, so familiar, right? We still import React, but you'll notice we also import **Core Components** from React Native too. We have a HelloWorldApp component rendered as usual, and the only other thing that should look weird is the use of `<Text>` rather than, say, a `<h1>` tag or a `<p>` tag. 

Let's have a look at some more.


```
import React from 'react';
import { StyleSheet, Text, View } from 'react-native';

export default function App() {
  return (
    <View style={styles.container}>
      <Text>
       Open up App.js to start working on your app!
      </Text>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center',
  },
});
``` 

You can see that we've imported StyleSheet from react-native for styles that target multiple elements (like using classes), and that we can also do inline styling, like in React. 

Here you can also see we have the `<Text>` tag from the last example, as well as a `<View>`. A View is basically the equivalent of a `<div>` in HTML. 

### Views

A View is a fundamental component for creating a UI with React Native. In development on Android and iOS, a native view is the basic building block of UI: a small rectangular element on the screen which can be used to display text, images, or respond to user input. 

Just like divs, views can contain other views, and things like buttons, lines of text and images are all examples of kinds of views in mobile development.

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646835035131/pxw4D2-1K.png)

*Source: https://reactnative.dev/docs/intro-react-native-components#views-and-mobile-development*

A React Native View is equivalent to a native View on iOS or Android, i.e. a UIView in iOS, or an android.view in Android. Views support Flexbox by default, as well as styles and touch events.

Here's a table showing the equivalence between the most common React Native Views (known as Core Components), the native views, and the web analogs (HTML tags). You can think of them as React Native's "translation" of the native components. 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646835307063/KpwmHfN7D.png)

Android and iOS have different native components, which means they might render slightly differently, even if they both use the same React Native code. For example, in the image below you can see the different application of the same shadow style, with the elements displayed in their unique, platform-specific manner. 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646836359910/WVVUmoCvI.png)

If the slight differences are an issue, you can manually override the styling by applying a sprinkling of Platform specific code:

```
import {Platform, StyleSheet } from 'react-native';

const styles = StyleSheet.create({
   container: {
      flex: 1,
      ...Platform.select({
         ios: {
            backgroundColor: 'red'
         },
         android: {
            backgroundColor: 'green'
         },
         default: {
         // other platforms, e.g. web
            backgroundColor: 'blue'
         }
      })
   }
});

```

### Web Views

As well as core components, React Native can also render custom components (like the `HelloWorldApp` component we saw in a previous example), and web views. 

A Web View is like an embeddable browser that a native app can use to display web content. 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646835574765/qOr_mCNxq.png)

You can think of it as a web-friendly island floating in an ocean of nativeness. The contents of the island don't have to be local to the app, as they can be pulled from a remote internet server. 

This can have performance issues, compared to rendering platform components, as the content needs to be loaded from elsewhere. 

However, there are many reasons why web views are used:

- Easier to update - just edit your web code and the web view updates because it pulls it down fresh every time.
- Useful if you have a web app already and want to use some of that in your mobile app without rewriting it to use native code.

### Testing Mobile Apps

You can run mobile app code on an emulator on your computer, which looks a lot like this:

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646835800976/qWCqLjQJ1.png)

You can also wire up a physical mobile device to your PC and get your app code to load on a real phone. 

However, while you can certainly build your React Native app for both operating systems using the same code, to test the code, you need to do this separately for the different operating systems. To test on iOS, you need an iOS emulator or device. To test your code works on Android, you need to test on an Android emulator or device. 

The program you use to spin up an emulated Android device, Android Studio, is available on all OSs. Apples puts a bit of a spanner in the works by not allowing its equivalent program, XCode to be used on non-Apple devices. 

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646836036058/04Wh3S2co.png)

This means that if you are not a Mac user, you can only test your React Native code on Android devices. To test on iOS, you either need to procure a Mac so that you can install XCode or get a subscription to a "Mac in a Cloud" (a virtual machine). 

This last option is what I do at work. It's not great for development, because the machine is a bit laggy, and you can't customise it easily (e.g. to use your bash aliases, set up nice colours in your terminal etc). However, it does the job for shallow testing and debugging small issues. 

This is why you might find advice on the internet saying that Macs are better for developing mobile apps on, because you can test both major operating systems on them at once. 

### My experience as a Junior with React Native

Summarising my first couple of months with React Native, here are my main takeaways:

- **Mobile emulators are cool!** There's something really fun about having a full-functioning mobile screen on your PC. You can use the camera, tilt the screen, delve into the device settings to find dark mode, etc. 

- **React Native documentation is great!** A lot of this post was heavily borrowed from their website, so go and check it out!

- **Debugging is way more tricky than on web.** In web development, I'm very used to using the console and developer tools for debugging CSS and network requests. There seems to be a lot less of this kind of tooling in the mobile world. The console equivalents and debugging tools that I found were unreliable, tricky to use and didn't have the whole picture. I'm going to keep trying to figure them out though, and this will probably be my next blog post! Stay tuned...

![image.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1646837077014/_YdLO4sPZ.png)

- **Setup can be complicated**, especially if you're not on a Mac. The documentation recommends using Expo (a dev server for watching changes), but for one reason or another that wasn't suitable at my workplace. My setup involved installing the Java development kit, Android development environment (including Android Studio, a virtual device, the SDK platform...), setting various environment variables, etc. Be prepared for this to take a while! 

- **The admin around the Play Store/Apple Store looks like a faff!** I haven't been directly involved in this so far, but from what I can see, you have to jump through a lot of hoops to get your code out there. It also seems less democratic, and is certainly a far cry from the wide and open web where anyone can chuck their code up and have it viewed across the world instantly for free. At the end of the day, Google and Apple make money of these things, so their stores are a bit of a paywall.

### Wrap Up

Hopefully that gives you a bit of an intro into React Native, and how to develop on mobile when you come from a web dev background! Feel free to comment or ask any questions, and please HMU if you know of any better debugging techniques! :)

