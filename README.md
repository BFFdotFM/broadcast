# BFF.fm Broadcast Server

This repo contains BFF.fm's [Azuracast](https://azuracast.com/) Liquidsoap 2.1 configuration.

Since we deployed Azuracast at the start of the pandemic, complementing our existing infrastructure (e.g. Google Workplace which we use for identity, and Creek which we use as our CMS, schedule, and playlist source-of-truth), we've bolted and duck-taped into Azuracast quite heavily at the Liquidsoap level, while also not wanting to lurch too far outside of Azuracast's great built-in features, because it's really good software that we could use more in the future.

While there's quite a lot of cross-dependency, hopefully you'll find these little pieces of module code useful, or educational since Liquidsoap's OCaml syntax can be quite tricky to learn.

## Features

* Library functions for HTTP operations with wrappers for JSON and form posting
* Logging to Slack webhooks
* Last.FM scrobbling
* TuneIn AIR posting
* Date/time functions
* Wrapper for handling multiple prioritised Icecast ingestion HTTP harbors, with ranking, metadata resolution, Slack status logging.
* Example of streamer authentication using an external API
* Some likely quite gnarly code — we learned on the job! Patches welcome!

## Support

If you find this useful, please consider donating to support BFF.fm's community radio operation in San Francisco:

* https://bff.fm/donate

And, of course, please consider donating to support ongoing development of Azuracast itself:

* https://docs.azuracast.com/en/contribute/donate
