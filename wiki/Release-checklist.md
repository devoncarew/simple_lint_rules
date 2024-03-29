# Release checklist

> [!IMPORTANT]
> The contents of this doc were copied from our wiki and have not yet been
> confirmed to be current and up-to-date. When this doc is next reviewed and
> updated please remove this comment.

# Release Candidate (full release)

For a release candidate leading up to a stable release, remember to:

1. Post to Dart Announce ([1.13 sample](https://groups.google.com/a/dartlang.org/forum/#!topic/announce/_d8SpOQX6jE))

# Stable release (full release)

For each full stable release, remember to:

### Documentation
1. Changelog reviewed to make sure everything is included
1. After the release, verify that https://api.dart.dev is serving the latest version

### Ecosystem
1. Validate that homebrew (macOS) and chocolatey (Windows) have been updated.

### Announcing

1 week before the final release, or approximately when we cut an RC0,
draft the following:

1. Publish blog post
1. Email changelog to announce@dartlang.org, and include a link to the blog post
1. Tweet
1. G+ post with link to blog post

When the release is out, publish the announcements and ask @googledev to reshare.

### Book keeping

1. Close milestone in github

# Stable release patch 

For each stable patch release -- e.g. 1.12.0 to 1.12.1 -- remember to:

1. Prior to creating the final build, update [CHANGELOG.md](https://github.com/dart-lang/sdk/blob/master/CHANGELOG.md) to mention the fixes (see 1.13.1 and 1.13.2 for examples)
1. Post an email to Dart Announcements ([announce@dartlang.org](https://groups.google.com/a/dartlang.org/forum/#!forum/announce))

