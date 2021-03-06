## Changelog

### 0.7.3 (2018-08-14)

* Add `registry_password_file` option to the config file.
* Improve no data message on empty tables on UI.
* Show the root namespace "library" in the dropdown even when there are no repos in it.
* Switch alpine Docker image to 3.8.

### 0.7.2 (2018-07-30)

* Make web root accessible w/o trailing slash when base_path is configured.

### 0.7.1 (2018-07-18)

* Fix panic when using MySQL for events storage and no table created yet.

### 0.7 (2018-07-04)

* When using MySQL for events storage, do not leak connections.
* Last events were not shown when viewing a repo of non-default namespace.
* Support repos with slash in the name.
* Enable Sonatype Nexus compatibility.
* Add `base_path` option to the config to run UI from non-root.
* Add built-in cron feature for purging tags task.

### 0.6 (2018-05-28)

* Add MySQL along with sqlite3 support as a registry events storage.
  New config settings `event_database_driver`, `event_database_location`.
* Bump Go version and dependencies.

### 0.5 (2018-03-06)

* Initial public version.
