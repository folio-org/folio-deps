# folio-deps

Copyright (C) 2025-2026 The Open Library Foundation

This software is distributed under the terms of the Apache License,
Version 2.0. See the file "[LICENSE](LICENSE)" for more information.

# Content

This repository lists all maven dependencies for each java module that is in any of the
[supported FOLIO flower release](https://docs.folio.org/docs/about-folio/support/)
or in the next flower release.

Only the latest released FOLIO module version for a flower release is listed.

It uses `mvn dependency:tree` without `-Dverbose` option so that a dependency this is used
multiple times is listed only once. Only the dependency path that results from dependency mediation
is listed: https://maven.apache.org/guides/introduction/introduction-to-dependency-mechanism.html

When the [FOLIO Security Team](https://folio-org.atlassian.net/wiki/spaces/SEC/overview) needs to find
vulnerable FOLIO modules for a given vulnerability of a maven library the team uses this repositories'
GitHub code search.

A manually triggered [GitHub Actions workflow](.github/workflows) updates the files.
