## How to contribute to OpenSSL

(Please visit https://www.openssl.org/community/getting-started.html for
other ideas about how to contribute.)

Development is done on GitHub, https://github.com/openssl/openssl.

To request new features or report bugs, please open an issue on GitHub

To submit a patch, please open a pull request on GitHub.  If you are thinking
of making a large contribution, open an issue for it before starting work,
to get comments from the community.  Someone may be already working on
the same thing or there may be reasons why that feature isn't implemented.

To make it easier to review and accept your pull request, please follow these
guidelines:

    1. Anything other than a trivial contribution requires a Contributor
    License Agreement (CLA), giving us permission to use your code. See
    https://www.openssl.org/policies/cla.html for details.  If your
    contribution is too small to require a CLA, put "CLA: trivial" on a
    line by itself in your commit message body.

    2.  All source files should start with the following text (with
    appropriate comment characters at the start of each line and the
    year(s) updated):

        Copyright 20xx-20yy The OpenSSL Project Authors. All Rights Reserved.

        Licensed under the OpenSSL license (the "License").  You may not use
        this file except in compliance with the License.  You can obtain a copy
        in the file LICENSE in the source distribution or at
        https://www.openssl.org/source/license.html

    3.  Patches should be as current as possible; expect to have to rebase
    often. We do not accept merge commits, you will have to remove them
    (usually by rebasing) before it will be acceptable.

    4.  Patches should follow our coding style (see
    https://www.openssl.org/policies/codingstyle.html) and compile
    without warnings. Where gcc or clang is available you should use the
    --strict-warnings Configure option.  OpenSSL compiles on many varied
    platforms: try to ensure you only use portable features.  Clean builds
    via Travis and AppVeyor are required, and they are started automatically
    whenever a PR is created or updated.

    5.  When at all possible, patches should include tests. These can
    either be added to an existing test, or completely new.  Please see
    test/README for information on the test framework.

    6.  New features or changed functionality must include
    documentation. Please look at the "pod" files in doc for
    examples of our style.
