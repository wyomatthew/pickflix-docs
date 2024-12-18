# Getting Started

So you'd like to get started watching media on Pickflix? You're in the right
place!

## What is Pickflix? ❓

It's a self-hosted streaming service powered by free, open-source software! The
core user experience is to request media via the request portal, wait for the
request to be fulfilled, and then stream the request via the streaming portal.
That's all you need to proceed, but feel free to refer to the [FAQ](faq.md) for
more information.

## Applications

### [Wizarr](https://welcome.pickflix.mov) 🔮

Wizarr (yes, two r's) handles all user onboarding. Before you can interact with
any other services, you'll need valid credentials, and Wizarr is how you'll get
them. If you're reading this, you should have already received an invite link
via Wizarr that looks something like <https://welcome.pickflix.mov/i/ABCDEF>.

Remember, Pickflix is an *invitation-only* service! Without this invitation, you
cannot start using Pickflix.

### [Jellyseerr](https://requests.pickflix.mov) 🖥️

Jellyseerr (yes, also two r's) processes all user requests. You can think of
Jellyseerr like IMDB: it's a massive metadata store of all the world's media.
Just about any movie or show to air can be found and requested on Jellyseerr.

### [Jellyfin](https://streaming.pickflix.mov) 🍿

Jellyfin is the where you'll go to actually stream media that's been requested
and fulfilled. This is your Netflix: you'll download the app on your phone, tv,
tablet, or wherever else you'd like and start watching.

## Onboarding Procedure 📋

Before proceeding, you should have already received an invite link that looks
something like <https://welcome.pickflix.mov/i/ABCDEF>. If so, press on!

1. Follow your invitation link in the browser

   Paste the link into your favorite browser and follow the instructions given
   to you by Wizarr. When you're done, you should have selected a username,
   entered a password, and joined the Discord for announcements.

2. Make your first request

   In your browser of choice, navigate to <https://requests.pickflix.mov>. When
   prompted, enter the credentials you created in step 1. Once authenticated,
   search for anything you'd like, click "Request", and finalize the request on
   the following pop up.

   Note at anytime you can navigate back to the piece of media you originally
   requested and monitor its progress.

3. Install Jellyfin

   While that request is being fulfilled, set up your streaming client. The
   process here will change depending on where you'd like to watch your media,
   so refer to
   [How do I install Jellyfin on X?](faq.md#how-do-i-install-jellyfin-on-x-) for
   more information. The easiest way to get started immediatey is to simply
   stream from the browser by navigating to <https://streaming.pickflix.mov>.

   Depending on your client, you may be prompted for a server address/host/etc.
   You should enter <https://streaming.pickflix.mov>. Regardless of your
   Jellyfin client, you'll authenticate using the same credentials created in
   step 1. Once authenticated, you should be able to browse the existing
   collection of fulfilled requests.

Just like that, you're done! You know how to request media and where to watch
it. Good job! 😎
