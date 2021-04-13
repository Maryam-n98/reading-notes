# Reading The Past, Present, and Future of Local Storage for Web Applications

"Persistent local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions."
Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. 
They have three potentially dealbreaking downsides:
1.Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
2.Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
3.Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful
Our goals is:
1.a lot of storage space
2.on the client
3.that persists beyond a page refresh
4.and isn’t transmitted to the server

Before HTML5, all attempts to achieve this were ultimately unsatisfactory in different ways.

"A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5:

In the beginning, there was only Internet Explorer. Or at least, that’s what Microsoft wanted the world to think. To that end, as part of the First Great Browser Wars, Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, Internet Explorer. One of these things was called DHTML Behaviors, and one of these behaviors was called userData."
**userData**  allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. 
Trusted domains, such as intranet sites, can store 10 times that amount. And hey, 640 KB ought to be enough for anybody.

##### INTRODUCING HTML5 STORAGE
What I will refer to as ***HTML5 Storage*** is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out into its own specification for uninteresting political reasons.
 Certain browser vendors also refer to it as ***Local Storage*** or ***DOM Storage.*** The naming situation is made even more complicated by some related, similarly-named, emerging standards that I’ll discuss later in this chapter.

You can write a storege function or Instead of writing this function yourself, you can use Modernizr to detect support for HTML5 Storage, it will be inside if.
"The storage event is supported everywhere the localStorage object is supported, which includes Internet Explorer 8. IE 8 does not support the W3C standard addEventListener (although that will finally be added in IE 9). Therefore, to hook the storage event, you’ll need to check which event mechanism the browser supports. (If you’ve done this before with other events, you can skip to the end of this section. Trapping the storage event works the same as every other event you’ve ever trapped. If you prefer to use jQuery or some other JavaScript library to register your event handlers, you can do that with the storage event, too.)"
