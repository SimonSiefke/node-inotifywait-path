# node-inotifywait-path

Prebuilt [inotifywait](https://github.com/inotify-tools/inotify-tools) binary for usage in nodejs.

## Install

```
$ npm inotifywait-path
```

## Usage

```js
import { inotifyWaitPath } from "inotifywait-path";
import { spawn } from "child_process";

// same as inotifywait -r -m /tmp/myFolder
const childProcess = spawn(inotifyWaitPath(), ["-r", "-m", "/tmp/myFolder"], {
  stdio: "inherit",
});
```

## License

MIT, but the downloaded `inotifywait` binary is licensed under [GNU General Public License v2.0](https://github.com/inotify-tools/inotify-tools/blob/master/COPYING)
