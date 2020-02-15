### ===== 0.9.0 =====
 - Complete rewrite of the build script to support multiple SBC
 - Migrate from debian jessie to buster
 - Switch form tuktuk to freeboard-sk
 - Many many theming changes
 - Pypilot now run under it's own user. 
 - limited sudo access for signalk
 - webapp are now served localy via nativfier
 - mDNS resolve for http://lysmarine.local 
 - Switched from fbi to plymouth for boot screen. 
 - Desactivate many unused .service for faster boot time (it's now around 12sec in a RPI3B+) 
 - Add build for PineA64
 - Add build for Vbox drive image.

### ===== 0.8.2 =====
 - Add create_ap to support wifi access point mode (CLI only)
 - Fix pypilot & add menu entry.
 - Switch form wicd to nm
 - Rename x11vnc service to vnc
 - Improve documentation

### ===== 0.8.1 =====
 - Regroup all web services under /var/www/
 - Global install of the npm package
 - Add conky
 - Disable RDP. See (https://gitlab.com/lysmarine/lysmarine/issues/23)
 - Improve stage organisation in the build script
 - Improve documentation

### ===== 0.8.0 =====
 - Original release
