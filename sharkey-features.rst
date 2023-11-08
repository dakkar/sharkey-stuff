Sharkey vs Misskey
==================

A (probably comprehensive) list of differences
----------------------------------------------

Big ones
""""""""

* fully federated note editing, you can also see previous versions of
  edited notes
* Mastodon-compatible API, including OAuth2
* admins can require approval for new users' signups
* admins can silence users
* admins can mark all of a user's media as NSFW
* GDPR-style Data Subject Access Requests (users can export all data
  related to themselves)

Fun ones
""""""""

* can play module / tracker music files
* (federated) listenbrainz integration
* (federated) background image on user profiles
* "speak as cat" separate from "is a cat" (both setting are federated
  with compatible software)

UI/UX
"""""
  
* option to open a note's detailed view by clicking on the note (most
  useful on mobile)
* images lacking alt text are marked as such
* UI elements can be round (as in Misskey) or square-ish
* "sign out" button in settings
* user profile page has "notes" / "all" / "including files" tabs
* attachments can be collapsed by default
* buttons to show/hide all notes with CWs in a conversation
* one-button "like" (plus custom reactions on a separate button)
* animated MFM can be enabled/disabled on each note
* supports longer alt text
* pop-up user profiles show if follow requests to the user require
  approval
* MFM cheatsheet when composing notes
* it's always clear if a note has a poll (misskey sometimes hides
  that)
* boosts and quote-boost are accounted separately
* only 1 boost plus 1 quote-boost per note per user is allowed
* admins can remove bots from "trending"
* users can hide bots from their timelines
* translatable notes are shown translated regardless of where they're
  shown (e.g. when quoted, or when looking at their replies)
* when searching, users can restrict results to notes with attachments
* CSS class names are human-readable, to simplify browser-side
  customisation
* users can disable indexing of their notes (the setting is federated)

Ones of interest to admins
""""""""""""""""""""""""""

* quote-boosts federate correctly from/to Mastodon forks
* better compatibility with relays
* support keydb as an alternative to redis
* the not-very-functional "automatically mark attachments as NSFW" has
  been removed (smaller installation, faster image/video uploads)
* argon2 instead of bcrypt for hashing users' secrets
* admins can delete remote emojis
* admins can disable achievements
* admins can refresh remote user details
