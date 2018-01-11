# dmonitor
Displays a live stream of one or more running containers’ resource usage statistics with the container name
## Install
To install, change directory to the location you want to download the script directory.  Use git to pull or clone this script into directory.  If you do not have git then enter; "sudo apt-get install git".  On the github page of this script use the "HTTPS clone URL" with the 'git clone' command.

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
    
#### System OS script tested
 * Ubuntu 14.04.3 LTS

#### Design Principles
 * Have a simple setup process and a minimal learning curve
 * Be usable as non-root
 * Be easy to install and configure
 
## License::

Permission is hereby granted, free of charge, to any person obtaining a copy of this software, associated documentation, and files (the "Software") without restriction, including without limitation of rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE. IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
