# FAQ

## How does Pickflix work?

That's a big question! At a high level, requests are made against a big database
of media (think something like [IMDB](https://www.imdb.com/)). This database
contains information *about* the media but not the actual movies or shows
themselves. Once a user has requested something, a separate application will
search through a list of trusted sources for a network that hosts the request.
Once a network is found, it will piece together the actual content from several
peers in the network. The assembled result is then stored and made available for
streaming.

For more detailed information, see the [Technical Guide](technical-guide.md).

## Is Pickflix safe to use?

Yes! Your client is simply a media player: it retrieves data from the server and
plays it on your display. Even if someone malicious were able to manipulate the
data sent to your client, it would recogize the payload doesn't constitute a
valid piece of media and fail. For furthe reassurance, even before the data
reaches your client, it is processed for integrity by server.

## I know someone who would love Pickflix! Can I share my credentials with them?

Depends. Using the same credentials within the same household (say, with your
partner and family) is totally fine!

If considering sharing credentials with several folks outside your home, I
kindly ask you *do not*. It's important for keeping the service stable that we
have a good approximation of the real number of human users, which is unbalanced
if many humans use a single account. Also, being able to moderate against abuse
requires I know the chain of people through which somebody is accessing the
platform, which is impossible with credential sharing.

But, if you know someone excited by Pickflix, then Pickflix would be excited to
have them as a user! Refer to
[How can I invite someone to Pickflix](#how-can-i-invite-someone-to-pickflix)
for more info.

## How can I invite someone to Pickflix?

This is a feature I'm actively working on! However, for the time being there is
no way for users to extend an invite for someone else to join Pickflix. Until
implemented, simply reach out to me and I will be able to generate a link for
them to sign up!

## My Jellyfin client wants a server address. What do I enter?

<https://streaming.pickflix.mov>

## How do I install Jellyfin on X?

Well, it depends on X! In general, any device with access to an app store will
have a client available for you to watch Jellyfin. If you're wondering if your
particular device is supported, then the latest collection of clients can always
be found directly on Jellyfin's website at <https://jellyfin.org/downloads/>
(don't forget to toggle "Recommended" to "All" if you don't see your device!).
Below are some particular recommendations from other Pickflix users:

- Desktop (Windows/MacOS/Linux)

  Jellyfin maintains an official desktop client that supports all platforms.
  Follow instructions for installation here:
  <https://github.com/jellyfin/jellyfin-media-player>.

  If you want to make life even easier, you can always watch from your favorite
  browser at <https://streaming.pickflix.mov>.

- Mobile (Android)

  Jellyfin maintains an official Android client that works very well. You can
  find it in the Google Play store, Amazon appstore, or F-Droid by searching for
  "Jellyfin".

  The unofficial client [Streamyfin](https://www.streamyfin.app/) is another
  option that users have reported good things about. Simply search for
  "Streamyfin" in the Google Play store.

- Mobile (iOS)

  Jellyfin maintains an official iOS client that is mostly feature complete.
  Mixed feedback has been reported on offline download support, but everything
  else works great. You can find it in the App Store by searching for
  "Jellyfin".

  If you're unsatisfied with the official client,
  [Streamyfin](https://www.streamyfin.app/) also supports iOS devices and is
  reported to have better support for offline downloads. It can also be found in
  the App Store by searching for "Streamyfin".

- Smart TV (Android)

  Whether your TV is an integrated Android TV or you have a separate Android TV
  that connects to your TV via HDMI (like an Nvidia SHIELD etc), it should have
  access to the Google Play store. Jellyfin maintains an official Android TV
  client that is quite stable, but you may experience instability depending on
  how powerful your device is. Regardless, simply search for "Jellyfin" in the
  Google Play store and install.

- Roku

  Jellyfin maintains an official client for Roku devices that is very stable.
  You can find it in the Channel Store by searching for "Jellyfin".

  Note the following from the Jellyfin official client:

  > Due to a technical limitation of the Roku store, the Jellyfin app for Roku
  > may state that a cable or satellite subscription is required. However, no
  > subscription of any form is required to use the Jellyfin server or any
  > official client.

- Smart TV (Apple)

  Apple TVs do not have an official Jellyfin client. You should first try
  Swiftfin, an unofficial client. You can find it in the App Store by searching
  "Swiftfin". Audio sync issues have been reported in the past on some media
  setups, so consider using a different client if you experience audio desync.

  Apple TVs can also try [Infuse](https://firecore.com/infuse). It is a
  proprietary media player, but advertises free support for Jellyfin. Users have
  reported an irritating experience as Infuse advertises its subscription model,
  but you should be able to use it if you can get past the pop-ups.

  If you don't have any luck with the two options above, sorry! You should check
  if the underlying TV that you plug your Apple TV into supports any of the
  other options mentioned above.

- Casting

  Any device that supports casting (such as a Google Chromecast) can also stream
  content from Pickflix by installing the mobile client mentioned above and
  simply casting the media. Nice!
