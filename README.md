# IllumiDesk

This is the IllumiDesk docs repo. Docs are managed with [Mkdocs](http://www.mkdocs.org/).

There are two options available to use 3Blades:

- [IllumiDesk](https://illumidesk.com) is available online with a free trial period. No credit card required.

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

    git remote add upstream https://github.com/illumidesk/docs

    > Sync upstream master with your fork using `git fetch upstream master` and `git merge upstream/master` to avoid merge conflicts.

5. Test site locally:

    mkdocs serve

6. Push to your fork and create PR

7. Merges to upstream master trigger a deploy to `https://docs.illumidesk.com`

## Documentation

- [Issue tracking](https://github.com/illumidesk/docs/issues)
- [Documentation](https://docs.illumidesk.com/)

## Copyright and license

Copyright © 2016-2017 3Blades, LLC. All rights reserved, except as follows. Code
is released under the BSD 3.0 license. The README.md file, and files in the
"docs" folder are licensed under the Creative Commons Attribution 4.0
International License under the terms and conditions set forth in the file
"LICENSE.docs". You may obtain a duplicate copy of the same license, titled
CC-BY-SA-4.0, at http://creativecommons.org/licenses/by/4.0/.
