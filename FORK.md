This fork carries the live ADB position fix for Home Assistant.

Android reports a position anchor plus speed and an update timestamp measured
against device uptime. Read uptime together with the media-session dump, advance
valid playing anchors to the sample time, preserve paused positions, and expose
the matching UTC timestamp to Home Assistant. No duration or metadata is invented.

Upstream base: e41603250834175bad4bd9b2f7c3352ec66f9707
Upstream: https://github.com/parkercombes/ha-google-tv-streamer

Install this fork through HACS instead of the upstream repository, not alongside
it: both use the google_tv_streamer domain. Keep this fork selected until the fix
is merged upstream. The Home Assistant TV template itself remains separate.
