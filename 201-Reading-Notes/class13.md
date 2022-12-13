# 201 Class 13 Reading Notes

## Summary: This class is about local storage and How To Use It On Websites

Why would a developer use local storage for a web application?
-caching data from the Web when it takes a long time to get it.
-Another use case is to store the state of interfaces.

What information should not be stored in local storage?

-Should not record user actions and information without the user’s knowledge

Local storage can store what type of data? How would you convert it to that type before storing?

## Working Around The “Strings Only” Issue

-shortcoming of local storage is that you can only store strings in the different keys. This means that when you have an object, it will not be stored the right way.
-work around this by using the native JSON.stringify and JSON.parse methods:

[Source:] <https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/>

## Bookmark/Skim

“The Past, Present, and Future of Local Storage for Web Applications”

## Things I want to know more about
