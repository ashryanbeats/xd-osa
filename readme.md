# xd-osa

An Applescript that reloads XD plugins and then runs a plugin.

# Usage

Command line:

```
$ osascript /path/to/script.scpt "{your_plugin_label}"
```

Or, from xdpm's `install.js` you can:

```
const cmd = `osascript /path/to/script.scpt "{your_plugin_label}`;
require("child_process").exec(cmd, function(error, stdout, stderr) {
  if (error) console.log(error);
});
```

Doing something like this, you can achieve an "autoreload" effect for your plugin.

# Praise for xd-osa

> We’re getting close to resurrecting animals like the woolly mammoth—but should we?
>
> - [Dr. Lynn J. Rothschild](https://qz.com/1566083/we-shouldnt-bring-back-extinct-animals-like-the-woolly-mammoth/), Astrobiologist at NASA's Ames Research Center

> Your scientists were so preoccupied with whether or not they could, they didn’t stop to think if they should.
>
> - Dr. Ian Malcolm, Jurassic Park
