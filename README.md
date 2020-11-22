View Unpublished
======================

The View Unpublished module adds the missing permissions `"view unpublished
$content_type content"` to Backdrop.

This module also integrates with the core Content overview screen at
/admin/content. If you choose the "not published" filter, Backdrop will show you
unpublished content that you're allowed to see.

Installation
------------

- Install this module using [the official Backdrop CMS
instructions](https://backdropcms.org/guide/modules).

- Visit the permissions page under Administration > Configuration > User
Accounts > Permissions (admin/config/people/permissions) and select the content
types to give view permission to.

Documentation and Common Issues
-------------

If using `view_unpublished` with Views, use the "Published or admin" filter, NOT
"published = yes". Views will then respect your custom permissions.

If for some reason this module does not seem to work, try rebuilding your node
permissions at admin/reports/status/rebuild. Note that this can take significant
time on larger installs and it is HIGHLY recommended that you back up your site
first.

Note that block caching is disabled for modules that implement
`hook_node_grants` (like this one). There are workarounds: see [this
issue](https://drupal.org/comment/8647155#comment-8647155) for one possibility
(for the Drupal version of this module). See also [Block Cache
Alter](https://drupal.org/project/blockcache_alter) for another possible
approach.

Additional documentation is located in [the
Wiki](https://github.com/backdrop-contrib/view-unpublished/wiki/Documentation).

Differences from Drupal 7
-------------------------

The "View any unpublished content" permission is now part of Backdrop core and
so has been removed from this module.

Issues
------

Bugs and feature requests should be reported in [the Issue
Queue](https://github.com/backdrop-contrib/view-unpublished/issues).

Current Maintainers
-------------------

- [Robert J. Lang](https://github.com/bugfolder).

Credits
-------

- Ported to Backdrop CMS by [Robert J. Lang](https://github.com/bugfolder).
- Originally written for Drupal by [Domenic Santangelo
(entendu)](https://www.drupal.org/u/entendu).

License
-------

This project is GPL v2 software.
See the LICENSE.txt file in this directory for complete text.

