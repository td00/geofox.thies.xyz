# simple gti.geofox.de dashboard page

`index.html` is just a few iframes containing the actual php pages rendering the connections

the php files (`busse.php`, `einwaerts_s3.php`, `einwaerts_s31.php` & `auswaerts.php`) show the actual connections.

A little bit of bootstrap css and a `dark.css` file allow for a dark background to look prettier on a status board.

The frames reload every 10 seconds.

# Requirements

- git.geofox.de credentials
- php-xml
- php-curl
- webserver (nginx/apache2/caddy)

# Documentation
## Status
- ![](https://raw.githubusercontent.com/td00/geofox.thies.xyz/main/assets/images/green.png) => Live tracking available & everythings in order
- ![](https://raw.githubusercontent.com/td00/geofox.thies.xyz/main/assets/images/red.png) => cancelled
- ![](https://raw.githubusercontent.com/td00/geofox.thies.xyz/main/assets/images/grey.png) => no live information available
- ![](https://raw.githubusercontent.com/td00/geofox.thies.xyz/main/assets/images/yellow.png) => delayed
- ![](https://raw.githubusercontent.com/td00/geofox.thies.xyz/main/assets/images/black.png) => delayed (in a traffic jam)
## Setup
Clone the git repo to your web folder, copy `inc\credentials.php.example` to `inc\credentials.php` and replace the user & password with the provided credentials.

If you don't have the required credentials, you'll need to go to https://www.hvv.de/fahrplaene/abruf-fahrplaninfos/datenabruf/ to request API credentials.

# Credits & License

Based on [axaneco/hvvclient](https://github.com/axaneco/hvvclient)

Licensed under [GNU General Public License v3.0](LICENSE)
