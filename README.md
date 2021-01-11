# grafanatomatoes
Grafana Config and Dashboard for Top DVD &amp; Streaming on Rotten Tomatoes

![Dashboard Picture](https://github.com/DennisFaucher/grafanatomatoes/blob/main/tomatoes_dashboard.png)

I have been adding Plex stats to my latest Grafana dashboard and thought an updated list of new DVD & streaming would be a nice add. Since Rotten Tomatoes is not giving our API keys any longer, I searched around and found [this great site](https://pypi.org/project/rotten_tomatoes_client/) on a "public API". I played with the examples and the instructions in the code until I had the correct JSON URL.

## Installation
* Install the Telegraf/InfluxDB/Grafana stack
* Add tomatoes.conf to /etc/telegraf/telegraf.d directory
* Test with "telegraf --config /etc/telegraf/telegraf.d/tomatoes.conf --test"
* Restart telegraf
* Add a new panel in your Grafana dashboard and use the 
