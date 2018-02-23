ROADMAP
=======

0.6.0 (unreleased)
------------------


0.5.0 (unreleased)
------------------
- [ ] vtalks/web : [Create a client test to check a random talk detailed view anon users](https://github.com/vtalks/vtalks.net/issues/60)
- [ ] vtalks/web : [Create a client test to check home anon users](https://github.com/vtalks/vtalks.net/issues/59)
- [ ] vtalks/web : [talks.models.Playlist to its own application](https://github.com/vtalks/vtalks.net/issues/92)
- [x] vtalks/web : [talks.models.Channel to its own application](https://github.com/vtalks/vtalks.net/issues/91)
- [x] vtalks/web : [Create a 500 template](https://github.com/vtalks/vtalks.net/issues/86)
- [x] vtalks/web : [Create a 404 template](https://github.com/vtalks/vtalks.net/issues/85)


0.4.0 (2018-02-07)
------------------
- [x] vtalks/web : [Content syndication](https://github.com/vtalks/vtalks.net/issues/48)
- [x] vtalks/web : [Apply unique_together = ('user', 'talk') on talk_likes](https://github.com/vtalks/vtalks.net/issues/76)
- [x] vtalks/web : [Apply unique_together = ('user', 'talk') on talk_dislikes](https://github.com/vtalks/vtalks.net/issues/77)
- [x] vtalks/web : [Apply unique_together = ('user', 'talk') on talk_favorites](https://github.com/vtalks/vtalks.net/issues/78)
- [x] vtalks/web : [Create robots.txt file](https://github.com/vtalks/vtalks.net/issues/65)
- [x] vtalks/web : [Better template contact form](https://github.com/vtalks/vtalks.net/issues/55)
- [x] vtalks/web : [Create a sitemap.xml for vtalks.net](https://github.com/vtalks/vtalks.net/issues/58)
- [x] vtalks/twitter-worker : [Add tags on the twitter content](https://github.com/vtalks/twitter_worker/issues/1)
    - [x] vtalks/web : [Add tag support for API talks](https://github.com/vtalks/vtalks.net/issues/83)

0.3.0 (2018-01-29)
------------------
- [x] vtalks/web : [Implement dislike talk by users](https://github.com/vtalks/vtalks.net/issues/47)
- [x] vtalks/web : [Implement favorite talk by users](https://github.com/vtalks/vtalks.net/issues/46)
- [x] vtalks/web : [Update rank on talk save](https://github.com/vtalks/vtalks.net/issues/45)
- [x] vtalks/deploy : [Add postgres adminer image](https://github.com/vtalks/deploy/issues/1)
- [x] vtalks/web : [Use DEBUG=False in production](https://github.com/vtalks/vtalks.net/issues/25)
- [x] vtalks/web : [Support for pagination on add_playlist management command](https://github.com/vtalks/vtalks.net/issues/24)


0.2.0 (2018-01-27)
------------------
- [x] Add support for coveralls.io.
    - [x] Minimum of 75% coverage.
- [x] Readonly API.
    - [x] List support for model Channel.
    - [x] List support for model Playlist.
    - [x] List support for model Talk.
    - [x] Details view support for model Channel.
    - [x] Details view support for model Playlist.
    - [x] Details view support for model Talk.
    - [x] Get Random Talk 
- [x] Read/Write API.
    - [x] Create support for model Channel.
    - [x] Create support for model Playlist.
    - [x] Create support for model Talk.
    - [x] Update support for model Channel.
    - [x] Update support for model Playlist.
    - [x] Update support for model Talk.
- [x] Add/Deploy NATS as a broker.

0.1.0 (2018-01-14)
------------------
- [x] Basic listing of talks.
- [x] Detailed view of a talk.
- [x] Search talks.
- [x] Twitter Authentication.
- [x] Basic ranking algorithms.
- [x] Basic UI and templates.
- [x] Readonly public API.
- [x] Initial set of tests and documentation.


## Backlog

The [backlog](https://github.com/issues?user=vtalks) is where all issues 
(including bugs, questions and enhancements) can be found. 

This list is the most updated source of work todo on the project.


## Ideas

This is a list of not yet planed and/or implemented ideas for vtalks.net. 
Before start working on the following, they should be researched and a set of
issues must be created on the backlog.

The idea is finished only when all of its issues are closed.

The current ideas are:

- Talks should have an optional link to their slides.
- Speaker model.

