tumblr theme for sleepingcatsyndrome.com
========================================

# Usage

1. input your tumblr account

```
$ vi ./myTheme/.peakconfig.yml
output_path: .peak
port: 1235
index: index.html
blog: kuronekomichael
email: michael@cat.email.ne.jp
password: ******
```

2. launch server and edit html

```
$ npm install
$ cd theme
$ ../node_modules/.bin/peak watch
```

# dev tool: [Peak](https://github.com/nporteschaikin/peak)

https://github.com/nporteschaikin/peak  
https://github.com/kuronekomichael/peak/

# Known Issues

- [x] watch only displaying {block:Photo}'s \#20  
https://github.com/nporteschaikin/peak/issues/20  
https://github.com/kuronekomichael/peak/commit/bc667e92eb6e7b64afb14444c2e158a9c93e090a

- [ ] `peak watch --path ./theme` is not work  
e.g, `watch --path /path/to/theme/`  
Compiler is success, but web server is blank.  
Maybe Peak haven't referenced to `options.output_path` to `--path`.

# TODO

- [ ] Enable infinite scrolling
- [ ] Enable code coloring
