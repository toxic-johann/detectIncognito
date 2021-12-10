# detectIncognito.js
detectIncognito.js can be used to detect incognito mode & other private browsing modes on most modern browsers as of December 2021.

 * Detects Incognito mode on Google Chrome
 * Detects Private Windows on Safari for macOS
 * Detects Private Tabs on Safari for iOS
 * Detects Private Windows in Firefox
 * Detects InPrivate Windows on Microsoft Edge
 * Detects InPrivate Windows on Microsoft Internet Explorer
 * Detects Private Windows in Brave

DEMO: https://detectincognito.com/

# Supported Browsers
 * Safari for iOS - 8 to 15
 * Safari for macOS <= 15
 * Chrome/Chromium - 50 to 96
 * Edge - 15 to 18; 79 to 96
 * Firefox - 44 to 95
 * MSIE >= 10
 * Brave <= 1.32

Please note that although this script works on almost all modern browsers, detecting private modes in browsers is very much an arms race. As such, I cannot guarantee that this script will continue to work into the future. However, I will continue to actively maintain this script to support as many browsers as is possible.

If you are aware of any modern browsers this script does not work with, please let me know by creating an issue.

# Changelog
 v21.12.0 - Dec 10, 2021 (mandatory)
 * [*] Chrome Fix: fixed Chrome using usage instead of quota
 * [*] The callback now returns an object instead of a boolean. obj.isPrivate will now return the status of private mode.
 * [+] The callback now includes the browser name as obj.browserName.

# Notes
 * This script does not detect Container Tabs on Firefox as they work differently compared to private mode.
 * An error will be thrown if the browser cannot be identified.
 * The script only works remotely (i.e. on a web server). Running the script locally may produce a false result, or not run at all.
 * [Issue #3](https://github.com/Joe12387/detectIncognito/issues/3 "Issue #3"): The script may cause a false result in certain automated testing scenarios.
