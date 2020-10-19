# dmonitor
[![GitHub Stable Release](https://img.shields.io/badge/Release-1.2-blue.svg)](https://github.com/BradleyA/dmonitor/releases/tag/1.2)
![GitHub Release Date](https://img.shields.io/github/release-date/BradleyA/dmonitor?color=blue)
[![GitHub Commits Since](https://img.shields.io/github/commits-since/BradleyA/dmonitor/1.2?color=orange)](https://github.com/BradleyA/dmonitor/commits/)
[![GitHub Last Commits](https://img.shields.io/github/last-commit/BradleyA/dmonitor.svg)](https://github.com/BradleyA/dmonitor/commits/)

[![Open GitHub Issue](https://img.shields.io/badge/Open-Incident-brightgreen.svg)](https://github.com/BradleyA/dmonitor/issues/new/choose)
[![GitHub Open Issues](https://img.shields.io/github/issues/BradleyA/dmonitor?color=purple)](https://github.com/BradleyA/dmonitor/issues?q=is%3Aopen+is%3Aissue)
[![GitHub Closed Issues](https://img.shields.io/github/issues-closed/BradleyA/dmonitor?color=purple)](https://github.com/BradleyA/dmonitor/issues?q=is%3Aclosed+is%3Aissue)

[<img alt="GitHub Clones" src="https://img.shields.io/static/v1?label=Clones&message=98&color=blueviolet">](https://github.com/BradleyA/dmonitor/blob/master/images/clone.table.md)
[<img alt="GitHub Views" src="https://img.shields.io/static/v1?label=Views&message=411&color=blueviolet">](https://github.com/BradleyA/dmonitor/blob/master/images/view.table.md)
[![GitHub Size](https://img.shields.io/github/repo-size/BradleyA/dmonitor.svg)](https://github.com/BradleyA/dmonitor/)
![Language Bash](https://img.shields.io/badge/%20Language-bash-blue.svg)
[![MIT License](http://img.shields.io/badge/License-MIT-blue.png)](LICENSE)

----

Displays a live stream of one or more running containers’ resource usage statistics with the container name

#### If you like this repository, select in the upper-right corner, star, thank you.

## Install
To install, change directory to the location you want to download the script directory.  Use git to pull or clone this script into directory.  If you do not have git then enter; "sudo apt-get install git" if using Ubuntu.  On the github page of this script use the "HTTPS clone URL" with the 'git clone' command.

    git clone https://github.com/BradleyA/dmonitor.git
    cd dmonitor

Move the script or create a symbolic link to a location in your working path; example /usr/local/bin. To find directories in your working path use; "echo $PATH".

    sudo ln -s $PWD/dmonitor /usr/local/bin/dmonitor

## Usage
    dmonitor

## Output
    CONTAINER                 CPU %               MEM USAGE / LIMIT   MEM %               NET I/O               BLOCK I/O
    compose3_nginx_1          0.01%               3.121 MB / 4 GB     0.08%               36.27 kB / 19.97 kB   0 B / 0 B
    compose3_redis_1          0.01%               6.57 MB / 4 GB      0.16%               18.44 kB / 648 B      0 B / 0 B
    compose3_web1_1           0.81%               29.8 MB / 4 GB      0.75%               22.66 kB / 5.402 kB   0 B / 0 B
    compose3_web2_1           0.68%               27.98 MB / 4 GB     0.70%               21.17 kB / 4.203 kB   0 B / 0 B
    compose3_web3_1           0.71%               27.98 MB / 4 GB     0.70%               20.58 kB / 4.245 kB   0 B / 0 B
    private-registry          0.00%               26.57 MB / 4 GB     0.66%               198.4 kB / 648 B      43.93 MB / 0 B
    prometheus_cadvisor_1     2.67%               31.57 MB / 4 GB     0.79%               211 MB / 7.785 GB     0 B / 0 B
    prometheus_exporter_1     0.00%               909.3 kB / 4 GB     0.02%               3.162 kB / 648 B      0 B / 0 B
    prometheus_promdash_1     0.01%               99.11 MB / 4 GB     2.48%               112.4 kB / 2.73 MB    0 B / 0 B
    prometheus_prometheus_1   0.03%               250.9 MB / 4 GB     6.27%               128.5 MB / 14 MB      0 B / 3.695 GB

#### Author
[<img id="github" src="images/github.png" width="50" a="https://github.com/BradleyA/">](https://github.com/BradleyA/)    [<img src="images/linkedin.png" style="max-width:100%;" >](https://www.linkedin.com/in/bradleyhallen) [<img id="twitter" src="images/twitter.png" width="50" a="twitter.com/bradleyaustintx/">](https://twitter.com/bradleyaustintx/)       <a href="https://twitter.com/intent/follow?screen_name=bradleyaustintx"> <img src="https://img.shields.io/twitter/follow/bradleyaustintx.svg?label=Follow%20@bradleyaustintx" alt="Follow @bradleyaustintx" />    </a>

#### System OS script tested
 * Ubuntu 14.04.3 LTS (amd64,armv7l)
 * Ubuntu 16.04.3 LTS (armv7l)

#### Design Principles
 * Have a simple setup process and a minimal learning curve
 * Be usable as non-root
 * Be easy to install and configure
 
#### License
MIT License

Copyright (c) 2020  [Bradley Allen](https://www.linkedin.com/in/bradleyhallen)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
