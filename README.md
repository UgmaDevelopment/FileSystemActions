FileSystemActions
=================

Provides a configurable Windows Service leveraging the FileSystemWatcher, to perform actions when a directory or file is created, changed, renamed or deleted.

#Configuration example

```xml
<?xml version="1.0" encoding="utf-8" ?>
<watchers>
  <watcher>
    <action event="onCreated" command="onCreated.bat" />
    <action event="onChanged" command="onChanged.bat" />
  </watcher>
  <watcher>
    <action event="onRenamed" command="onRenamed.bat" />
    <action event="onDeleted" command="onDeleted.bat" />
  </watcher>
</watchers>
```