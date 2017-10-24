[![slack in](https://slack.3blades.io/badge.svg)](https://slack.3blades.io)

# 3Blades

This is the 3Blades docs repo. Docs are managed with [Mkdocs](http://www.mkdocs.org/).

There are two options available to use 3Blades:

- [Online](https://3blades.io): cloud version with free trial period. No credit card required.
- [On-premises](https://github.com/3blades/onpremise): free community version available. Pro version adds more goodies and support services.

And yes, 3Blades is open source, **BSD 3-Clause** licensed!

## Docs Setup

1. Fork this repo
2. Clone and cd into your fork

    git clone https://github.com/<github_account_name>/docs
    cd docs

3. To setup docs clone this repo and install requirements. We recommend using [virtualenv](https://virtualenv.pypa.io/en/stable/):

    virtualenv venv
    source venv/bin/activate
    pip install -r requirements.txt

4. (Optional) Add remote upstream

    git remote add upstream https://github.com/3blades/docs

    > Sync upstream master with your fork using `git fetch upstream master` and `git merge upstream/master` to avoid merge conflicts.

5. Test site locally:

    mkdocs serve

6. Push to your fork and create PR

7. Merges to upstream master trigger a deploy to `https://docs.3blades.io`


## Documentation

- [Community](https://slack.3blades.io)
- [Issue tracking](https://github.com/3Blades/docs/issues)
- [Documentation](https://docs.3blades.io/)

## Copyright and license

Copyright © 2016-2017 3Blades, LLC. All rights reserved, except as follows. Code
is released under the BSD 3.0 license. The README.md file, and files in the
"docs" folder are licensed under the Creative Commons Attribution 4.0
International License under the terms and conditions set forth in the file
"LICENSE.docs". You may obtain a duplicate copy of the same license, titled
CC-BY-SA-4.0, at http://creativecommons.org/licenses/by/4.0/.
