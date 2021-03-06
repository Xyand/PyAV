We are operating with semantic versioning <http://semver.org/>. However,
we are using v0.x.y as our heavy development period, and will increment `x`
to signal a major change (i.e. backwards incompatibilities) and increment
`y` as a minor change (i.e. backwards compatible features).


0.2.4
=====
- fix library search path for current Libav/Ubuntu 14.04 (#97)
- explicitly include all sources to combat 0.2.3 release problem (#100)


0.2.3
=====

WARNING: There was an issue with the PyPI distribution in which it required
Cython to be installed.

Major:
- Python IO.
- agressively releases GIL
- add experimental Windows build (#84)

Minor:
- several new Stream/Packet/Frame attributes

Fixes:
- fix segfault in audio handling (#86 and #93)
- fix use of PIL/Pillow API (#85)
- fix bad assumptions about plane counts (#76)


0.2.2
=====
- Cythonization in setup.py; mostly a development issue.
- Fix for av.InputContainer.size over 2**31.


0.2.1
=====
- Python 3 compatibility!
- Build process fails if missing libraries.
- Fix linking of libavdevices.


0.2.0
=====

WARNING: This version has an issue linking in libavdevices, and very likely
will not work for you.

It sure has been a long time since this was released, and there was a lot of
arbitrary changes that come with us wrapping an API as we are discovering it.
Changes include, but are not limited to:

- Audio encoding.
- Exposing planes and buffers.
- Descriptors for channel layouts, video and audio formats, etc..
- Seeking.
- Many many more properties on all of the objects.
- Device support (e.g. webcams).


0.1.0
=====
- FIRST PUBLIC RELEASE!
- Container/video/audio formats.
- Audio layouts.
- Decoding video/audio/subtitles.
- Encoding video.
- Audio FIFOs and resampling.
