View Unpublished
----------------
This small module adds the missing permissions "view any unpublished content"
and "view unpublished $content_type content" to Drupal 7.

Using view_unpublished with Views
---------------------------------
Use the "Published or admin" filter, NOT "published = yes". Views will then
respect your custom permissions. Thanks to hanoii (6.x) and pcambra (7.x) for
this feature.


Releated isses on drupal.org
----------------------------
[New node permission "view any unpublished content"](http://drupal.org/node/273595)
[Enable Node Grants for Unpublished Nodes](http://drupal.org/node/452538)


Thanks to:
----------
Florian Weber (webflo) and thekevinday for their work on the D7 port.