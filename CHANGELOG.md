
Version 2.2.2 (2021-08-16)
--------------------------
Fix crash on tvOS caused by access to filesystem (#621)
Fix Session UserID not consistent among tracker instances (#630)

Version 2.2.1 (2021-08-02)
--------------------------
Fix build errors in Xcoce 13 beta 3 when using SPM (#628)

Version 2.2.0 (2021-07-16)
--------------------------
Remove Demo app builds for iOS 12 on CI (#626)
Set amended v_tracker indicating wrapper tracker version (#624)
Set application install timestamp on device timestamp field (#625)
Avoid deprecated method for configuration serialization (#623)
Fix for CaseSensetive file systems (#622) (Contribution of @Juraldinio)

Version 2.1.1 (2021-06-24)
--------------------------
Fix Gdpr context being tracked without enabling it (#618)

Version 2.1.0 (2021-06-18)
--------------------------
Fix sessionIndex starting from 0 rather than 1 (#616)
Fix missing base64encoding in remote config (#615)
Fix screenView autotracking unable to send events (#614)
Fix tvOS integration via SwiftPM unable to compile (#611)
Bump FMDB to version 2.7 (#612)
Fix Swift names clash for SelfDescribing event (#610)
Fix data race accessing currentScreenState (#609)
Add remote configuration (#581)

Version 2.0.2 (2021-05-24)
--------------------------
Add geolocation to SubjectConfiguration and SubjectController (#604)
Fix duplicate NS_SWIFT_NAME macro (#603)
Fix IDFA not accessible on iOS 14 (#601)

Version 2.0.1 (2021-05-12)
--------------------------
Fix crash if data from Database is corrupted (#596) (Contribution of @glukhanyk)
Add SubjectController to update userId (#595)
Fix NSInvalidArgumentException on first run with v2.0 (#592)
Fix macOS target for SPM (#593) (Contribution of @Juraldinio)

Version 2.0.0 (2021-04-27)
--------------------------
Set lifecycle tracking off by default (#587)
Update README (#502)
Fix GitHub Actions failures due to redirection to macos-10.15 (#583)
Remove protocol from NetworkController and NetworkConnection (#573)
Add custom headers for requests (#364)
Store sessions info separately per tracker namespace (#570)
Add API reference documentation for configurations and controllers (#568)
Add NSDictionary as explicit argument in SPSelfDescribingJson (#274)
Allow multiple instances of the tracker (#566)
Import corrections from Android tracker (#563)
Create API for v.2.0 (#558)
Restructure project source tree (#552)
Bump deployment target to iOS 9 (#550)

Version 1.7.0 (2021-04-03)
--------------------------
Fix issue of OpenIDFA causing App Rejection (#575)

Version 1.6.2 (2021-01-12)
--------------------------
Fix internal Carthage issues with Xcode 12.3 (#561)
Fix leak on SNOWReachability (#559) (Contribution of @i-dama)

Version 1.6.1 (2020-11-24)
--------------------------
Fix AddGlobalContext unable to work when GlobalContexts not initialized (#553)
Let Crash reporting to add contexts and AppID (#555)
Fix Snyk script (#549)
Move demo apps to snowplow-objc-tracker-examples (#547)

Version 1.6.0 (2020-09-21)
--------------------------
Update GitHub Actions to test on iOS 14 (#545)
Enable Xcode 12 support for Swift Package Manager (#544) (Contribution of @lunij)
Session storageMechanism is marked SQLITE but it's not (#482)
Make session uuid rotation dependant on events being tracked (#497)

Version 1.5.0 (2020-09-01)
--------------------------
Crash connected with method writeSessionToFile in SPSession (#515)
Emitter refactoring (#540)
Report logs to the app (#534)
Add diagnostic feature (#533)

Version 1.4.1 (2020-07-22)
--------------------------
TrueTimestamp has to be set in seconds. (#532)
ScreenView event doesn't track transitionType (#516) 

Version 1.4.0 (2020-07-10)
--------------------------
Validate EventData in Unstructured events (#526)
Fix url percent escaping (#525)
Fix contexts duplication (#524)
Add method for setting true timestamp (#276)
Renew event ID when event object is reused (#521)
Move from Travis CI to GitHub Actions (#517)
Add unified track method for all the events (#518)

Version 1.3.1 (2020-05-07)
--------------------------
Remove SPM demo app as it causes issues to Carthage (#513)
Specifcy FMDB version instead of commit in Package.swift (#512) (Contribution of @BennetLinden)
Adds public access to a tracker's current session id (#508) (Contribution of @ejensen)
Add missing references to SPConsentDocument.h (#507) (Contribution of @ejensen)

Version 1.3.0 (2020-04-21)
--------------------------
Swift Package Manager unable to find headers on subfolders (#503) (Contribution of @vauxhall)
Replace deprecated CTTelephonyNetworkInfo methods (#479)
Fix deprecated CFURLCreateStringByAddingPercentEscapes (#493)
Fix deprecated keyWindow (#492)
Update Technical Docs link (#443)
Update copyright (#499)
Add GDPR context (#425)
Add support for global contexts (#357)
Add Swift Package Manager support (#474) (Contribution of @vauxhall)
Events processing refactoring (#489)

Version 1.2.2 (2020-03-04)
--------------------------
Fix failing test about ScreenContext (#486)
FMDB versions conflicts with other dependency (#432)

Version 1.2.1 (2020-02-12)
--------------------------
Fix screen context not correctly updated on screenView events (#483)

Version 1.2.0 (2020-01-20)
--------------------------
Ensure addDictionaryToPayload enumeration over immutable dictionary (#480) (Contribute of Matt Robinson)
Stop updating screen context when auto-tracking is disabled (#431)
Fix valueForKey error in auto-tracking for screenviews (#428)
Add Watchkit support (#465) (Contribute of Leo Mehlig)
Allow overwriting of the 'platform' parameter (#476)
ReachabilitySwift conflicts with Reachability (#437)

Version 1.1.5 (2019-11-25)
--------------------------
Fix travis script not able to test on iOS 13.2 (#472)
Fix IDFA rejection when app submitted with v.1.1.4 (#470)

Version 1.1.4 (2019-11-11)
--------------------------
Fix doc of method setTimestamp (#467)
Set simulator device model information when it runs on simulator (#468)
Update swift demo app for 1.1.4 (#460)
Update objc demo app for 1.1.4 (#461)
Fix Slather (#453)
SnowplowTracker-swift.h file not found static lib building (#427)
Fix building issues on MacOS target (#466)
Fix bridging issues importing the framework on swift demo app (#458)
Fix installation of SnowplowTracker via Carthage (#457)
Fix Nocilla at 0.11 (#455)
Comply with isAdvertisingTrackingEnabled (#447)
Fix incomplete device model information (#444)

Version 1.1.3 (2019-10-18)
--------------------------
Fix broken build process (#452)
Fix ReachabilitySwift at 4.3.1 (#449)

Version 1.1.2 (2019-05-16)
--------------------------
Fix Cartfile in SnowplowSwiftDemo (#420)
Fix SPError class name conflict with WatchKit (#418)
Fix podspec validation issues (#419)

Version 1.1.1 (2019-05-15)
--------------------------
Make SPScreenState.h public and foward declare in SPEvent.h (#415)
Fix recursion in screen auto-tracking (#416)

Version 1.1.0 (2019-05-06)
--------------------------
Allow configurable postPath parameter (#409)
Fix various build warnings (#414)
Fix warning about self references being retained in SPSession (#412)
Add tests for application context (#410)
Add automatic tracking of install lifecycle event (close #374)
Enable automatic unhandled exception tracking (#371)
Add automatic screen view events and screen context (#370)

Version 1.0.4 (2019-02-28)
--------------------------
Use NS_ENUM for SPRequestOptions and SPProtocol (#402)
Fix key-value order for application context (#406)

Version 1.0.3 (2019-02-25)
--------------------------
Remove unnecessary Reachability from podspec (#404)
Fix value reported by Reachability (#403)

Version 1.0.2 (2019-02-20)
--------------------------
Add Carthage badge (#390)
Lower minimum deployment targets (#399)
Update old badges (#400)

Version 1.0.1 (2019-02-20)
--------------------------
Update README.md for new documentation site (#394)
Update Swift demo Cartfile (#393)
Add initializers for SPSession (#396)
Remove dangling constant (#395)
Add Doxygen-generated API reference (#392)

Version 1.0.0 (2019-01-28)
--------------------------
Exposes session property in SPTracker (#256)
Fix parameter documentation (#389)
Make initializers unavailable in SPEmitter and SPTracker (#255)
Add OpenIdfa files to framework target (#382)
Resolve potential memory leaks from implicit retain of self (#353)
Embed Swift standard library for tests (#388)
Disable always embed Swift standard libraries (#381)
Remove exceptions (#383)
Explicitly close all statements in FMDB (#384)
Fix getDocuments function in consent events (#386)
Add support for Carthage (#291)
Replace Reachability with Reachability.swift (#385)

Version 0.9.0 (2018-10-15)
--------------------------
Fix ConsentGranted builder argument type in tests (#361)
Add SRCROOT to project header search path (#362)
Update pods committed to Git repo (#360)
Update CocoaPods in Travis build (#359)
Add application context capability (#358)
Commit IDEWorkspaceChecks.plist to repo (#354)
Add foreground and background events (#349)

Version 0.8.0 (2018-04-29)
--------------------------
Update CocoaPods to 1.4.0 and add pod update repo in build script (#347)
Add method to SPTracker to get session's userId (#345)
Drop iOS 8 test target, add iOS 10 and 11 (#344)
Fix SnowplowTests bundle custom folder name (#343)
Add a Swift port of SnowplowDemo (#342)
Add identifyUser as alias for setUserId (#341)
Add trackConsentGrantedEvent and trackConsentWithdrawnEvent methods (#340)
Remove "close" from CHANGELOG for issue #333 (#338)
Add support for push notification open tracking (#335)
Add preprocessor flags to disable OpenIDFA or IDFV (#334)
Extend copyright notice in all files to 2018 (#331)
Replace NSGregorianCalendar with NSCalendarIdentifierGregorian (#329)
Fix truncation of structured event value to 6 digits (#299)
Add trackSelfDescribingEvent method as alias for trackUnstructEvent (#272)

Version 0.7.0 (2017-12-24)
--------------------------
Bump iOS deployment target to 8.0 (#326)
Bump Xcode to 9.1 and test against iOS 8.1 and 9.0 (#325)
Bump CocoaPods to 1.3.1 (#306)
Bump FMDB to 2.6.2 (#315)
Use default Bundler version in Travis (#336)
Fix invalid latitude in test suite (#322)
Don't attempt to serialize nil object in event store (#286)
Fix method description typos (#317)
Update README markdown in accordance with CommonMark (#333)

Version 0.6.2 (2016-10-10)
--------------------------
Fix failing geolocation_context test (#293)
Cast from NS(U)Integer to long type causes crashes on 32-bit devices, thanks @chrisfsampaio (#271)
App crashes on iPhone 4s simulator, thanks @chrisfsampaio (#278)
Fix Travis build (#295)
Fix failing getLanguage test on Travis (#294)
Correct the capitalization of Xcode in README, thanks @ReadmeCritic (#268)

Version 0.6.1 (2016-02-22)
--------------------------
Made podfile dependencies more restrictive (#266)
Harmonized foreground and background timeouts with Android (#265)
Fixed Cast from NS(U)Integer to long type causing crashes on 32-bit devices (#264)
Fixed crash when logging emitter attempts, thanks @rockshassa! (#262)

Version 0.6.0 (2016-01-18)
--------------------------
ClientSession needs to send null for the first previousSessionId (#257)
Removed buffer limit in favour of only using bytelimit (#245)
Only start a single timer, be sure to stop previous checker (#252)
Updated Cocoapods version to 0.39.0 (#243)
Updated pauseEventTracking so that the emitter timer is invalidated/stopped (#218)
Changed floats, doubles and ints to NSNumbers (#96)
Added tvOS deployment target to Podspec (#244)
Added missing tickets to CHANGELOG (#226)
Added event class with builder options for all event types (#223)
Added tests to check generated self-describing jsons against their schemas in iglu (#222)
Added Precondition checks for Tracker and Emitter (#221)
Added option to set event id manually (#195)
Added firstEventId to client_session context (#194)
Added batching based on payload size (#162)
Added a SelfDescribingJson class to ensure we build contexts and unstructured events properly (#119)
Added preconditions to event builders to ensure they are setup correctly (#117)
Added location context information (#68)
iOS9 ATS issues with OpenIDFA (#175)
SPUtilities getLanguage returns country code appended string in iOS9 (#233)
Floats and doubles are not being correctly shortened to two decimal places (#232)
Ensured emitter url uses HTTPS for iOS9 (#231)
OpenIDFA calendar is deprecated for iOS 8, thanks @iamjason! (#230)
SPUtilities getTimestamp should return an NSInteger not double (#229)
Fixed classname collision: SPUtils vs WatchKit.framework, thanks @iamjason! (#228)
Fixed tvOS could not create database queue for path (#251)
Replaced legacy docset_url in podspec with documentation_url (#259)

Version 0.5.2 (2015-09-30)
--------------------------
Fixed regression of mobile_context to 1-0-0 from 1-0-1 (#235)
Fixed SessionIndex being passed as a string not as an integer (#234)
Fixed .gitignore to work with Xcode 7 (#241)

Version 0.5.1 (2015-09-11)
--------------------------
Added entropy to global constants to avoid clang errors with other libraries (closes #224)

Version 0.5.0 (2015-09-03)
--------------------------
Removed OCHamcrest test dependency from podfile (#211)
Validated all public properties of all classes (#209)
Simplified SPTracker event decoration into a single function (#204)
Configured SPSubject to match how other Tracker Subject classes function (#203)
Fixed SPUtils functions need to return nil not an empty string if they fail to get a value (#213)
Fixed SPUtils getPlatform function which only returns "mob" as a default string (#205)
Fixed RequestCallback has to import Foundation before defining protocol (#202)
Fixed Emitter timer must be setup on main thread or it will not run (#201)
Ensured platform is set as it is a required field for payload_data (#206)
Ensured that sendEvents will run in background only (#197)
Made RequestCallback protocol more idiomatic to obj-c (#189)
Changed "POST" and "GET" options to enums (#120)
Renamed initWithURLRequest to initWithURL (#114)
Updated test suite to cover all code in the tracker (#208)
Updated contexts schema to 1-0-1 (#207)
Updated all class namespaces (#200)
Updated payload-data to 1-0-3 (#91)
Created SnowplowConstant class or equivalent (#35)
Created an option to opt-out of data collection (#27)
Added Mocking library for proper unit testing of emitter requests (#212)
Added Tracker builder options to pass through session timeouts (#210)
Added synchronized mutex lock to emitter results to prevent BAD_ACCESS_ERR (#216)
Added an implementation of NSTimer without a strong reference to its parent target (#215)
Added option to set emitting thread pool size (#199)
Added option to set events to emit range (#198)
Added support for checking if the device is online before attempting to emit (#184)
Added a SnowplowSubject class equivalent to remove need to get same data over and over (#196)
Added `is online` label to the demo app (#193)
Added builder pattern for tracker/emitter (#190)
Added checks for malformed NSURL (#79)
Added in-client sessionization (#19)
Added device sent time on outbound events (#158)

Version 0.4.0 (2015-08-16)
--------------------------
Updated how the emitter sends information to match the Android Tracker flow (#185)
Full memory leak and performance analysis (#183)
Added functions to access metrics on the SQLite database (#182)
Added target for building Static iOS Framework, thanks @AlexDenisov! (#171)
Added iOS 6 support, thanks @agarwalswapnil! (#163)
Macroed out the usage of sharedApplication, thanks @hlian! (#157)
Added network properties implementation, thanks @duncan! (#142)
Added Coveralls code coverage to project (#108)
Added Mountebank for simple testing of tracker locally (#82)
Added support for callbacks for success/failure (#59)
Changed license in README to be pulled from CocoaPods (#130)
Using FIFO instead of "pending" flag to track emit progress (#94)
Made an iOS test app (#67)
Fixed Content-Type not being set correctly (#192)

Version 0.3.4 (2015-08-05)
--------------------------
Fixed Tracker sometimes POSTs when no events to post, thanks @leonardors! (#164)
Fixed bug in PR whereby POST is sent with many events when Buffer type is instant (#178)
Fixed FMDB requirement for an operation queue to work properly in a concurrent world (#179)
Fixed bug where appId is nullified if namespace is nil (#165)
Using buffer size to limit number of events per POST, thanks @leonardors! (#169)
Removed _buffer in SnowplowEmitter in favour of boolean counter (#173)
Removed extra DB queue layer for removing events (#181)

Version 0.3.3 (2015-03-26)
--------------------------
Fixed Travis button in README (#152) 	
Fixed the immediate flushing of the buffer (#153) 	
Fixed incorrect content type sent if GA SDK also running (#160)

Version 0.3.2 (2015-02-28)
--------------------------
Now using a querystring, not an HTTP body for GET, thanks @loufranco! (#141)
Removed unused ifdef around Base64 encoding, thanks @duncan! (#138)
Quieted unused variable warnings, thanks @duncan! (#139)
Quieted Gestalt method deprecation warnings, thanks @duncan! (#140)
Now unsetting payload key when value is nil, thanks @duncan! (#147)
Made SnowplowUtils public in podspec (#145)
Now using URL-safe Base64 without padding, thanks @loufranco! (#150)

Version 0.3.1 (2015-02-17)
--------------------------
Replaced SnowplowRequest.h with SnowplowEmitter.h as a public header, thanks @hamidp! (#133)
Excluded CoreTelephony dependency for OS X, thanks @duncan! (#134)
Removed AFNetworking dependency from podspec, thanks @duncan! (#136)
Adjusted logging to emit debug logs for Snowplow collector only when SNOWPLOW_DEBUG defined, thanks @atdrendel! (#131)

Version 0.3.0 (2015-02-15)
--------------------------
Reverted from AFnetworking to standard NSURLSession, thanks @atdrendel and @duncan! (#88)
Updated Travis to use the most up-to-date simulator (#90)
Cleaned up SnowplowTracker.podspec (#99)
Updated Podfile and re-installed to fix Travis (#93)
Renamed SnowplowRequest to SnowplowEmitter, thanks @jonalmeida! (#70)
Added new initializer with POST as default method, thanks @jonalmeida! (#69)
Updated getResolution test to allow 750x1334 for Retina iPhone (#92)
Added timings event (#89)
Added Mac OS X support, thanks @atdrendel and @duncan! (#104)
Renamed from snowplow-ios-tracker to snowplow-objc-tracker (#103)
Added License button to README (#109)

Version 0.2.2 (2014-12-18)
--------------------------
Added missing iglu: protocol for screen_view schema URI, thanks @michelmongkhoy! (#85)

Version 0.2.1 (2014-11-28)
--------------------------
Fixed unstructured events incorrectly sent wrapped in contexts schema (#81)

Version 0.2.0 (2014-11-08)
--------------------------
Only using IFA if AdSupport is included (#76)
Fixed XCode 6 compatibility (#77)

Version 0.1.2 (2014-09-28)
--------------------------
Fixed bug where UUIDs generated in uppercase, not lowercase (#71)
Applied temporary fix to Podfile for Travis builds (#73)

Version 0.1.1 (2014-09-10)
--------------------------
Fixed linting notes (#65)
Fixed screen view tracking using incorrect condition for nil id checking (#66)

Version 0.1.0 (2014-08-28)
--------------------------
Initial release
