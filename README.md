# Spotipy - a Python client for The Spotify Web API

## Description

Spotipy is a thin client library for the Spotify Web API.

## Documentation

Spotipy's full documentation is online at [Spotipy Documentation](http://spotipy.readthedocs.org/) 


## Installation
If you already have [Python](http://www.python.org/) on your system you can install the library simply by downloading the distribution, unpack it and install in the usual fashion:

    python setup.py install

You can also install it using a popular package manager with 

  `pip install spotipy`

or

  `easy_install spotipy`


## Dependencies

- [Requests](https://github.com/kennethreitz/requests) - spotipy requires the requests package to be installed


## Quick Start
To get started, simply install spotipy, reate a Spotify object and call methods:

    import spotipy
    sp = spotipy.Spotify()

    results = sp.search(q='weezer', limit=20)
    for i, t in enumerate(results['tracks']['items']):
        print ' ', i, t['name']

A full set of examples can be found in the [online documentation](http://spotipy.readthedocs.org/) and in the [Spotipy examples directory](https://github.com/plamere/spotipy/tree/master/examples).
        

## Reporting Issues

If you have suggestions, bugs or other issues specific to this library, file them [here](https://github.com/plamere/spotipy/issues). Or just send me a pull request.

## Version

- 1.0 - 04/05/2014 - Initial release
- 1.1 - 05/18/2014 - Repackaged for saner imports
- 1.4.1 - 06/17/2014 - Updates to match released API
- 1.4.2 - 06/21/2014 - Added support for retrieving starred playlists
- v1.40, June 12, 2014 -- Initial public release.
- v1.42, June 19, 2014 -- Removed dependency on simplejson
- v1.43, June 27, 2014 -- Fixed JSON handling issue
- v1.44, July 3, 2014 -- Added show tracks.py example
- v1.45, July 7, 2014 -- Support for related artists endpoint. Don't used cache auth codes when scope changes
- v1.49, July 23, 2014 -- Support for "Your Music" tracks (add, delete, get), with examples
- v1.50, August 14, 2014  -- Refactored util out of examples and into the main package
- v1.301, August 19, 2014 -- Upgraded version number to take precedence over previously botched release (sigh)
- v1.310, August 20, 2014 -- Added playlist replace and remove methods. Added auth tests. Improved API docs
- v2.0 - August 22, 2014 -- Upgraded APIs and docs to make it be a real library
- v2.0.01 - August 25, 2014 -- Moved to spotipy at pypi
