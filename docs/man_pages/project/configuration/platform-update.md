platform update
==========

Usage | Synopsis
------|-------
General |`$ tns platform update <Platform>[@<Version>]`
Android latest runtime |`$ tns platform update android`
Android selected runtime | `$ tns platform update android@<Version>`
<% if(isMacOS) { %>iOS latest runtime | `$ tns platform update ios`
iOS selected runtime | `$ tns platform update ios@<Version>` <% } %> 

Updates the NativeScript runtime for the specified platform.

### Attributes

* `<Platform>` is the target mobile platform whose runtime you want to update. You can set the following target platforms.
	* `android` - Updates the Android runtime.
	<% if(isMacOS) { %>* `ios` - Updates the iOS runtime.<% } %>
* `<Version>` is any available version of the respective platform runtime published in npm. <% if(isHtml) { %>If `@<Version>` is not specified, the NativeScript CLI installs the latest stable runtime for the selected platform.  
To list all available versions for Android, run `$ npm view tns-android versions`. To list only experimental versions for android, run `$ npm view tns-android dist-tags`  
To list all available versions for iOS, run `$ npm view tns-ios versions`. To list only experimental versions for ios, run `$ npm view tns-ios dist-tags` 

### Command Limitations

* You can run `$ tns platform update ios` only on OS X systems.

### Related Commands

Command | Description
----------|----------
[platform add](platform-add.html) | Configures the current project to target the selected platform.
[platform remove](platform-remove.html) | Removes the selected platform from the platforms that the project currently targets.
[platform](platform.html) | Lists all platforms that the project currently targets.
[prepare](prepare.html) | Copies common and relevant platform-specific content from the app directory to the subdirectory for the selected target platform in the platforms directory.
<% } %>