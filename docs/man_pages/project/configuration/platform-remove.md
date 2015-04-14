platform remove
==========

Usage | Synopsis
------|-------
General | `$ tns platform remove <Platform>`

Removes the selected platform from the platforms that the project currently targets. After removing the target platform, you can no longer build and deploy your app on devices which run on the platform.

<% if(isHtml) { %>This operation deletes the subdirectory for the selected platform from the platforms directory. <% } %>

### Attributes

`<Platform>` is the target mobile platform that you want to remove from your project. You can set the following target platforms.
* `android` - Removes configuration changes for Android development.
<% if(isMacOS) { %>* `ios` - Removes configuration changes for iOS development.<% } %>

<% if(isHtml) { %>
### Command Limitations

* You can run `$ tns platform remove ios` only on OS X systems.

### Related Commands

Command | Description
----------|----------
[platform add](platform-add.html) | Configures the current project to target the selected platform.
[platform update](platform-update.html) | Updates the NativeScript runtime for the specified platform.
[platform](platform.html) | Lists all platforms that the project currently targets.
[prepare](prepare.html) | Copies common and relevant platform-specific content from the app directory to the subdirectory for the selected target platform in the platforms directory.
<% } %>