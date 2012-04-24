Update !
========

- Deprecated, as this code had been added in Subscribe2 starting in v8 (the hooks were renamed)


Subscribe2 with new filters
===========================

This is simply a copy of WP Subscribe2 plugin, with 4 simple filters added:

- s2_send_plain_summary_suscribers
- s2_send_plain_fullcontent_suscribers
- s2_send_html_excerpt_suscribers
- s2_send_html_fullcontent_suscribers

These filters are called just before sending e-mails when a new post/article is published on the WordPress blog. (1 filter per e-mail type).

This allows to add/remove addresses on the fly right before the notifications are sent. All these functions will receive two parameters (see WP documentation about filters if necessary):

- the first is the array of recipients (e-mail addresses).
- the second is the post_id of the newly created post.

This makes possible, for example, to remove addresses of users if their preferred language is different of the Post language (you'll still need plugins to add multiligual features to WordPress).

