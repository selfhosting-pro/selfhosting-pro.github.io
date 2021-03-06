---
title: Plex vs. Jellyfin
date: 2022-06-05 15:27
categories: [multimedia]
tags: [plex,jellyfin]
---
# Plex vs Jellyfin
There are many media players that are suitable for streaming movies, series and music. Plex Media Server is certainly the top dog here, but there are alternatives. I would like to compare Plex vs. Jellyfin from my personal point of view. Of course, everyone must then decide for themselves which of the two programs they want to use.

## Why the comparison?
Surely it would be interesting for you to know why I compare Plex vs Jellyfin and why I don't include Emby or Kodi in the comparison. I can answer this question very easily:
I only use Plex and Jellyfin as media players. Admittedly, I have used Kodi, at that time still as XMBC a lot. But I simply see advantages here.

### Why not Kodi?
What does Plex vs Jellyfin have to do with Kodi in this post?
Kodi is set up differently compared to Plex, Jellyfin or Emby. Kodi is used as a direct media player on the end device, meaning here the media must be directly located or directly accessible via the network. The other tools are at home in a server-client infrastructure. Of course, this has its advantages and disadvantages.

### Advantages of Plex and Jellyfin over Kodi
I personally see these points as advantages. For someone else, they may well be a disadvantage. It's always the particular situation and/or intended use that needs to be evaluated.

For me, the server-client infrastructure has the advantage that I can offload the resources I need to the server. Possible transcoding is done on the more potent machine. This allows the client to be even a simpler Raspberry Pi.

Another advantage is that I can access my media on the go. Of course, the best way is always protected via VPN only.

### Disadvantages of Plex/Jellyfin/Emby compared to Kodi
You can reverse the advantages to get directly to the disadvantages. That means I don't need to run two devices here. If the media is on the same system as the player, you can save a lot of energy. If necessary, there is no need to buy a powerful system.

## Plex vs Jellyfin
Let's get to the actual comparison and the core of this post. I used Plex Media Server for many years to stream media from my server to playback devices on the TV or on the cell phone. Of course, all this time I also had a server that was already running 24/7, so no additional resources were needed.

Over the time I always used the free version of PMS. For the normal user this is fully sufficient. Then later the hardware transcoding was added and I really wanted to use this feature. So I had to use the Plex Pass. At that time, it only cost a few euros and was therefore quickly purchased. For the last few years, I have continued to pay by annual subscription, although a Black Friday deal would certainly have made the Plex Lifetime membership worthwhile.

With the Plex Pass you can do more than just hardware transcoding (you can now do that in the free version). Most will probably buy the feature to share his media library with friends and family. It also offers features like offline media availability. However, I have never really used both.

A few months ago, I just wanted to check out Jellyfin. I've heard a lot about it via podcasts, YouTube videos, and reddit, but never tried it. Jellyfin came about as a fork of Emby because a lot of people didn't like the way Emby was developing anymore and wanted to make it better.

Comparing Plex vs Jellyfin, the latter has the advantage that it is basically free and there is also no pay option. Of course, this has a certain disadvantage that development can't always go as fast as when a full time developer is working on the project.

![PlexVsJellyfin](/assets/images/plex-vs-jellyfin-watching-tv-1024x907.webp)
_Plex vs Jellyfin_

## What was bothering me about the Plex media server?
So why did I switch products? A lot had to do with my Kubernetes cluster at the time. Plex ran fine on it and I could very easily install Jellyfin in parallel and have a look. The user interface is definitely different, but can be configured per user at least somewhat. Here you don't have so many options with Plex.

When Plex had a problem with their server again and you can't log in to the system anymore, I was forced to consume my media via Jellyfin. You have to know that Plex has an online constraint. The media is streamed completely offline, but the client always logs in to the server via the cloud. Annoying when the infrastructure does not always work well.

Jellyfin still gives me the advantage of tracking my "watch history" cleanly on Trakt.tv (link to my profile). There are a few ways to do this via Plex, but they are often not maintained cleanly or require a paid Trakt.tv account.

I also like the playlists on Jellyfin better. For example, I have created lists for the Marvel Cinematic Universe to watch the movies again in order. The collections at Plex pack the movies together, but don't sort them in the correct order.

## What bothers me about Jellyfin
Comparing Plex vs Jellyfin, PMS has the charming advantage of having more supported clients. There is a native client for almost every operating system. For me in the Apple universe this was of course no problem.

Jellyfin on the other hand does not have an AppleTV client at the moment. Here you have to fall back on Infuse Pro. So now I have costs after all. Although much cheaper than Plex, but completely free I did not get.

The AndroidTV app is also rather bad than right (been). The old version had many bugs. With the current version, a lot of work has been done on it and now it runs very stable and performant.

## Conclusion
I feel more at home with Jellyfin than I did with Plex. Of course I still miss a native app for the AppleTV, but I can be content with the AndroidTV on the TV. On the iPhone or iPad I watch via Infuse Pro, because I already have the license.

The duel Plex vs Jellyfin wins for me, how could it be otherwise, Jellyfin. If you want to try out the software, you can have a look at my [Docker Compose collection](https://github.com/cbirkenbeul/docker-homelab), there you will find prefabricated files to get started.