### ISSUE: npm run test-local
1. egg-init 自动生成目录，选择 simple选项
2. 输入 egg-test-local 作为文件夹名称
3. 生成目录后，用 cnpm i 安装依赖包
4. npm run test-local

#### 报错情况如下：

```
$npm run test-local
> test-local@1.0.0 test-local /Users/cc/Documents/GitLinux/egg-test-local
> egg-bin test

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
npm ERR! code ELIFECYCLE
npm ERR! errno 1
npm ERR! test-local@1.0.0 test-local: `egg-bin test`
npm ERR! Exit status 1
npm ERR!
npm ERR! Failed at the test-local@1.0.0 test-local script.
npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

npm ERR! A complete log of this run can be found in:
npm ERR!     /Users/cc/.npm/_logs/2018-07-02T08_26_15_390Z-debug.log
```
