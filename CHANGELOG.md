# Changelog

## v1.1.0
- **Runs in the plugin worker runtime.** It now gets only what it asks for
  — `system:open` — and can't reach anything else in the app. Viboplr asks
  you to allow these once when you update. Requires Viboplr 1.0.85.
- Rebuilding the Search submenu after an edit relies on Viboplr 1.0.85, whose
  context-menu registry no longer lets a late unsubscribe remove the item that
  replaced it (in a worker, unsubscribes arrive a moment after re-registrations).

## v1.0.0
- Initial release. Externalized from the Viboplr app's built-in plugins (previously bundled as `search-providers`); functionally identical, now installable and updatable from the plugin gallery.
