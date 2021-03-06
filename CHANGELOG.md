# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)

## [0.2.19] - 2018-03-12

### Added

- Scroll bars are off by default
  https://github.com/thefrontside/frontmacs/pull/120

- Untabify and indent entire buffer if no region is selected
  https://github.com/thefrontside/frontmacs/pull/119

## [0.2.18] - 2018-02-09

### Changed

- Fix installation problem when emacswiki packages were taken
  offline. https://github.com/thefrontside/frontmacs/issues/115

## [0.2.17] - 2018-01-02

### Changed

- Fix api compatibility with `counsel-projectile`
  https://github.com/thefrontside/frontmacs/pull/95

## [0.2.15] - 2017-10-23

### Added
- default `rspec-use-rake-when-possible` to false. Rake just takes up
  a bunch of extra memory and computational power when invoked for
  little added benefit. Now when running rspec from emacs, it runs
  `bundle exec rspec` instead of `bundle exec rake spec`
- Add compilation regexes for node.js. Emacs doesn't know how to parse
  Node stack traces out of the box, so stack trace links aren't
  clickable or navigable with `goto-next-error`. Now they are.
