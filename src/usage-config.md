# Rclone Configuration


If you need to make specific changes to the rclone configuration and you dont want to use this apps user interface, this will explain how you can apply changes manually.

First you need to export your current config. Please refer to [this section about exporting.](usage-export.md#export)


After you have created your backup, transfer it to the pc of your choice. Then you need to extract all the files in the backup, you can use any program that can extract `.zip`-files.

The backup is structured the following way:

```
backup.zip
|-rcx.prefs
|-rcx.json
|-rclone.conf
```

Assuming you are in the folder where you extracted `rclone.conf` to, you can use the following command to edit the config with rclone.

`rclone --config ./rclone.conf config`

It is also possible to manually edit the configuration via text-editor.

When you made all those changes, transfer the configuration file back to your device. Please follow [the import guide](usage-export.md#eimport) to restore the changed config.


# Warning
With the upcoming overhaul, all available configuration options will be exposed via the UI. It should not be nessessary to edit the configuration in such a manner. There will be no support for changes made this way.