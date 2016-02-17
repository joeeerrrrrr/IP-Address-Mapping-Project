I was curious about illegal torrent litigation and file sharing, so I joined the swarm for some torrents and wrote all the peer information to a log file.

Regex was used to pull out IP addresses (it's rough right now, and needs to be refined). Then, the IP addresses were passed to the http://ipinfo.io/developers API which returns geo location information, among other things.

Then I used the Folium map package to mark IP locations. It was a challenge to find a map package that wasn't a ridiculous pain with dependencies and things like that but Folium seems very smooth, and works with different map services like OpenStreet and GoogleMaps.

I think tracking and mapping IP addresses can be useful for many applications in addition to plotting torrent peers. A tool to track and map IP addresses could be useful for marketing, advertising, mitigating DDoS attacks, or just better understanding demographics and who is using a particular service. So hopefully I can come back to this project later and expand on it.