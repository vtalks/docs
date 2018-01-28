ROADMAP
=======

0.6.0 (unreleased)
------------------


0.5.0 (unreleased)
------------------


0.4.0 (unreleased)
------------------
- [ ] vtalks/web : [Content syndication](https://github.com/vtalks/vtalks.net/issues/48)
- [x] vtalks/twitter-worker : Content syndication Twitter.
- [ ] vtalks/facebook-worker : Content syndication Facebook.
- [ ] vtalks/linkedin-worker : Content syndication LinkedIn.
- [ ] vtalks/docs : [Document virtualenv configuration on development](https://github.com/vtalks/docs/issues/3)
- [ ] vtalks/docs : [Use environment variables to configure the database](https://github.com/vtalks/docs/issues/2)


0.3.0 (unreleased)
-----------------
- [x] vtalks/web : [Implement dislike talk by users](https://github.com/vtalks/vtalks.net/issues/47)
- [x] vtalks/web : [Implement favorite talk by users](https://github.com/vtalks/vtalks.net/issues/46)
- [x] vtalks/web : [Update rank on talk save](https://github.com/vtalks/vtalks.net/issues/45)
- [ ] vtalks/web : [Send email contact form with mailgun](https://github.com/vtalks/vtalks.net/issues/44)
- [x] vtalks/deploy : [Add postgres adminer image](https://github.com/vtalks/deploy/issues/1)
- [x] vtalks/web : [Use DEBUG=False in production](https://github.com/vtalks/vtalks.net/issues/25)
- [ ] vtalks/web : [Support for pagination on add_playlist management command](https://github.com/vtalks/vtalks.net/issues/24)


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
- [ ] Periodically update outdated videos.
- [ ] Add Speaker model.
- [ ] API CRUD support for Speaker model.
- [ ] Add Conference/Event model.
- [ ] API CRUD support for Conference/Event model.
