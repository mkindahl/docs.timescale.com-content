# Deprecation Policy for TimescaleDB

TimescaleDB is an evolving system and over time features might become
obsolete or be replaced with new features. This means that some
options, functions, views, or other support for certain versions of
libraries or other software might have to be removed or replaced with
newer versions. In order to avoid breaking applications for users,
Timescale follow a formal deprecation policy to provide forward notice
of a planned breaking change.

1. Deprecations are announced in the release notes of a release and
   the release date counts as the deprecation announcement date.
2. Deprecation of a feature means that it might be removed in the next
   following major release.
3. Deprecation of a feature means that it will be supported for at
   least 12 months following the date the deprecation is annouced.

The deprecation policy only applies to GA releases: for alpha and beta
releases, we might have to change interfaces on a short notice and a
deprecation policy could potentially prevent us from improving
interfaces based on things we have learned during the beta
period. This would either affect the quality of TimescaleDB or create
longer beta periods than necessary.

The deprecation policy also only applies to breaking changes. API
changes that are forward compatible, such as adding new arguments to
functions or adding columns to views, are not considered breaking
changes and will not be handled using the deprecation policy.
