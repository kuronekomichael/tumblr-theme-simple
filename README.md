tumblr theme for sleepingcatsyndrome.com
========================================

# Usage

1. Input your tumblr account

```
$ vi ./theme/.peakconfig.yml
output_path: .peak
port: 1235
index: index.html
blog: kuronekomichael          <= sub-domain on tumblr.com (e.g, kuronekomichael.tumblr.com => kuronekomichael)
email: michael@cat.email.ne.jp <= tumblr account's email
password: ******               <= tumblr account's password
```

2. Edit html and Launch a local web server for tests

```
$ vi ./theme/index.html

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
Compiler is good, but web server is wrong.  
Maybe Peak haven't referenced to `options.output_path` to `--path`.

# TODO

- [ ] Enable infinite scrolling
- [ ] Enable code coloring
