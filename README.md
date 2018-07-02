### ISSUE: npm run test-local
1. egg-init 自动生成目录，选择 simple选项
2. 输入 egg-test-local 作为文件夹名称
3. 生成目录后，用 cnpm i 安装依赖包
4. npm run test-local (DEBUG=common-bin egg-bin test)

#### 报错情况如下：

```sh
$npm run test-local

> test-local@1.0.0 test-local /Users/cc/Documents/GitLinux/egg-test-local
> DEBUG=common-bin egg-bin test

  common-bin [EggBin] origin argument `test` +0ms
  common-bin [EggBin] add command `autod` from `/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/egg-bin/4.7.1/egg-bin/lib/cmd/autod.js` +5ms
  common-bin [EggBin] add command `cov` from `/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/egg-bin/4.7.1/egg-bin/lib/cmd/cov.js` +1ms
  common-bin [EggBin] add command `debug` from `/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/egg-bin/4.7.1/egg-bin/lib/cmd/debug.js` +0ms
  common-bin [EggBin] add command `dev` from `/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/egg-bin/4.7.1/egg-bin/lib/cmd/dev.js` +0ms
  common-bin [EggBin] add command `pkgfiles` from `/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/egg-bin/4.7.1/egg-bin/lib/cmd/pkgfiles.js` +0ms
  common-bin [EggBin] add command `test` from `/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/egg-bin/4.7.1/egg-bin/lib/cmd/test.js` +0ms
  common-bin [EggBin] loaded command `autod,cov,debug,dev,pkgfiles,test` from directory `/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/egg-bin/4.7.1/egg-bin/lib/cmd` +0ms
  common-bin [EggBin] dispatch to subcommand `test` -> `TestCommand` with [] +33ms
  common-bin [TestCommand] origin argument `` +1ms
  common-bin [TestCommand] exec run command +2ms
  common-bin Run fork `/usr/local/bin/node /Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/mocha/5.2.0/mocha/bin/_mocha --require=/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/egg-bin/4.7.1/egg-bin/lib/mocha-clean.js --require=/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/co-mocha/1.2.2/co-mocha/lib/co-mocha.js --require=/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/intelli-espower-loader/1.0.1/intelli-espower-loader/intelli-espower-loader.js --timeout=60000 --exit test/app/controller/home.test.js` +0ms
module.js:540
    throw err;
    ^

Error: Cannot find module '/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/intelli-espower-loader/1.0.1/package.json'
    at Function.Module._resolveFilename (module.js:538:15)
    at Function.Module._load (module.js:468:25)
    at Module.require (module.js:587:17)
    at require (internal/module.js:11:18)
    at getPackageJSON (/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/intelli-espower-loader/1.0.1/intelli-espower-loader/lib/get-package-json.js:29:12)
    at Object.<anonymous> (/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/intelli-espower-loader/1.0.1/intelli-espower-loader/intelli-espower-loader.js:3:44)
    at Module._compile (module.js:643:30)
    at Object.Module._extensions..js (module.js:654:10)
    at Module.load (module.js:556:32)
    at tryModuleLoad (module.js:499:12)
    at Function.Module._load (module.js:491:3)
    at Module.require (module.js:587:17)
    at require (internal/module.js:11:18)
    at requires.forEach.mod (/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/mocha/5.2.0/mocha/bin/_mocha:511:3)
    at Array.forEach (<anonymous>)
    at Object.<anonymous> (/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/mocha/5.2.0/mocha/bin/_mocha:510:10)
    at Module._compile (module.js:643:30)
    at Object.Module._extensions..js (module.js:654:10)
    at Module.load (module.js:556:32)
    at tryModuleLoad (module.js:499:12)
    at Function.Module._load (module.js:491:3)
    at Function.Module.runMain (module.js:684:10)
    at startup (bootstrap_node.js:187:16)
    at bootstrap_node.js:608:3
⚠️  Error: /Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/mocha/5.2.0/mocha/bin/_mocha --require=/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/egg-bin/4.7.1/egg-bin/lib/mocha-clean.js,--require=/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/co-mocha/1.2.2/co-mocha/lib/co-mocha.js,--require=/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/intelli-espower-loader/1.0.1/intelli-espower-loader/intelli-espower-loader.js,--timeout=60000,--exit,test/app/controller/home.test.js exit with code 1
⚠️  Command Error, enable `DEBUG=common-bin` for detail
  common-bin args  +185ms
  common-bin Error: /Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/mocha/5.2.0/mocha/bin/_mocha --require=/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/egg-bin/4.7.1/egg-bin/lib/mocha-clean.js,--require=/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/co-mocha/1.2.2/co-mocha/lib/co-mocha.js,--require=/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/intelli-espower-loader/1.0.1/intelli-espower-loader/intelli-espower-loader.js,--timeout=60000,--exit,test/app/controller/home.test.js exit with code 1
  common-bin     at ChildProcess.proc.once.code (/Users/cc/Documents/GitLinux/egg-test-local/node_modules/.npminstall/common-bin/2.7.3/common-bin/lib/helper.js:56:21)
  common-bin     at Object.onceWrapper (events.js:317:30)
  common-bin     at emitTwo (events.js:126:13)
  common-bin     at ChildProcess.emit (events.js:214:7)
  common-bin     at Process.ChildProcess._handle.onexit (internal/child_process.js:198:12) +0ms
npm ERR! code ELIFECYCLE
npm ERR! errno 1
npm ERR! test-local@1.0.0 test-local: `DEBUG=common-bin egg-bin test`
npm ERR! Exit status 1
npm ERR!
npm ERR! Failed at the test-local@1.0.0 test-local script.
npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

npm ERR! A complete log of this run can be found in:
...
```
