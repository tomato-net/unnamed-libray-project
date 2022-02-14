# Unnamed Library Project

A project to create software to improve the locating, downloading, converting, rating, cataologing books and ebook files.

## Plan

- Intergrate with Goodreads Connect to authenticate as a user and access their shelves
- Allow adding books to shelves
- Allow viewing of shelves
- Integrate with LibGen to find mirrors for book files for books in shelves
- Automatically convert those downloaded files to MOBI format or any desirable format
- Allow rating books and updating progress on books


## Questions

- What platform?
- Authenticated APIs?
    It's gonna be only used by us but needs some kind of user token so we can link goodreads tokens I assume, unless
    we just store all the data locally (local storage, file storage, etc)
- Where is the storage?
    Prefer local storage over server-side for cost reasons. Can allow backups of local storage somewhere, drive?
- Can we make it sync across devices?
    Probably not unless we do server storage which we're avoiding, so will most likely require backup and restore process
- Backups of storage?
    Use google drive on a schedule
- What kind of data do we need to store?
- Does LibGen have an API instead of storing a database?
- How does Goodreads Connect work?
- Do we want to store a cache of the shelves or do we want to request them from Goodreads API every time?
    Definitely want some cache, just do we want longterm or shortterm caching? How often do we request data from API?
- API limits on Goodreads API?
- Can we search LibGen by ISBN?


NEVER MIND, GOODREADS API HAS BEEN NUKED

So new plan, export into openlibrary account, use openlibrary as backend instead of goodreads
