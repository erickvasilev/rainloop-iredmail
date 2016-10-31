## rainloop-iredmail

A plugin for [RainLoop](http://www.rainloop.net) to allow your [iRedMail](http://www.iredmail.org) users to change their passwords. Tested on RainLoop 1.10.4 and iRedMail 0.9.5-1.

### Installation

This plugin supports both MySQL and PostgreSQL iRedMail editions. Sorry, no OpenLDAP.

1. Upload the "iredmail" directory to `data/_data_/_default_/plugins` in your RainLoop installation. (NOTE: Older versions of RainLoop have a slightly different data directory structure with a random hash, but you will still find a plugins directory)
2. Activate in the Plugins section of the admin area.
3. Configure with your iRedMail edition (MySQL/MariaDB or PgSQL), and the `vmail` database password iRedMail generated for you. You can find it in settings.py in iRedAdmin's root directory (`/opt/www/iredadmin`).
4. You may need to remove `escapeshellcmd` and `shell_exec` from PHP's disable_functions setting, in `/etc/php5-fpm/php.ini`.

If your iRedMail installation is modified enough to require such a change, the database hostname and other parameters can be edited in index.php.

This is an unofficial plugin with no affiliation to the iRedMail or RainLoop teams.

### License

Copyright (c) 2016, Jamie Hamilton  
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

  * Redistributions of source code must retain the above copyright
    notice, this list of conditions and the following disclaimer.

  * Redistributions in binary form must reproduce the above copyright
    notice, this list of conditions and the following disclaimer in the
    documentation and/or other materials provided with the distribution.

  * Neither the name of the author nor the names of its contributors
    may be used to endorse or promote products derived from this software
    without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL <COPYRIGHT HOLDER> BE LIABLE FOR ANY
DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND
ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
