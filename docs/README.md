---
title: 博客说明
tags:
    - Other
categories:
    - Other
---

## 版本说明
1. 基于Hexo, 主题为[hexo-theme-kidss]
2. 主要插件列表见备注中的组件树
3. hexo init后有调整相关目录结构，主要是和主题相关的软链接，以及调整写blog的markdown文件目录位置，并软链接到"source/\_posts"
4. 修改hexo-deploy-git库，增加将原markdown文件提交到github

---------------
## code style测试
    /*
     * test.c
     */
    #include <stdio.h>
    int main()
    {
        printf("hello world\n");
        return 0;
    }

---------------
## 备注
1. 组件树
        hexo-site@0.0.0
        ├─┬ hexo@3.2.2
        │ ├── abbrev@1.0.9
        │ ├── archy@1.0.0
        │ ├── bluebird@3.4.6
        │ ├─┬ chalk@1.1.3
        │ │ ├── ansi-styles@2.2.1
        │ │ ├── escape-string-regexp@1.0.5
        │ │ ├─┬ has-ansi@2.0.0
        │ │ │ └── ansi-regex@2.0.0
        │ │ ├── strip-ansi@3.0.1
        │ │ └── supports-color@2.0.0
        │ ├─┬ cheerio@0.20.0
        │ │ ├─┬ css-select@1.2.0
        │ │ │ ├── boolbase@1.0.0
        │ │ │ ├── css-what@2.1.0
        │ │ │ ├── domutils@1.5.1
        │ │ │ └── nth-check@1.0.1
        │ │ ├─┬ dom-serializer@0.1.0
        │ │ │ └── domelementtype@1.1.3
        │ │ ├── entities@1.1.1
        │ │ ├─┬ htmlparser2@3.8.3
        │ │ │ ├── domelementtype@1.3.0
        │ │ │ ├── domhandler@2.3.0
        │ │ │ ├── entities@1.0.0
        │ │ │ └─┬ readable-stream@1.1.14
        │ │ │   ├── core-util-is@1.0.2
        │ │ │   ├── isarray@0.0.1
        │ │ │   └── string_decoder@0.10.31
        │ │ └─┬ jsdom@7.2.2
        │ │   ├── abab@1.0.3
        │ │   ├── acorn@2.7.0
        │ │   ├── acorn-globals@1.0.9
        │ │   ├── cssom@0.3.1
        │ │   ├── cssstyle@0.2.37
        │ │   ├─┬ escodegen@1.8.1
        │ │   │ ├── estraverse@1.9.3
        │ │   │ ├── esutils@2.0.2
        │ │   │ ├─┬ optionator@0.8.2
        │ │   │ │ ├── deep-is@0.1.3
        │ │   │ │ ├── fast-levenshtein@2.0.5
        │ │   │ │ ├── levn@0.3.0
        │ │   │ │ ├── prelude-ls@1.1.2
        │ │   │ │ ├── type-check@0.3.2
        │ │   │ │ └── wordwrap@1.0.0
        │ │   │ └── source-map@0.2.0
        │ │   ├── nwmatcher@1.3.8
        │ │   ├── parse5@1.5.1
        │ │   ├─┬ request@2.75.0
        │ │   │ ├── aws-sign2@0.6.0
        │ │   │ ├── aws4@1.5.0
        │ │   │ ├─┬ bl@1.1.2
        │ │   │ │ └─┬ readable-stream@2.0.6
        │ │   │ │   └── isarray@1.0.0
        │ │   │ ├── caseless@0.11.0
        │ │   │ ├─┬ combined-stream@1.0.5
        │ │   │ │ └── delayed-stream@1.0.0
        │ │   │ ├── extend@3.0.0
        │ │   │ ├── forever-agent@0.6.1
        │ │   │ ├─┬ form-data@2.0.0
        │ │   │ │ └── asynckit@0.4.0
        │ │   │ ├─┬ har-validator@2.0.6
        │ │   │ │ ├─┬ commander@2.9.0
        │ │   │ │ │ └── graceful-readlink@1.0.1
        │ │   │ │ └─┬ is-my-json-valid@2.15.0
        │ │   │ │   ├── generate-function@2.0.0
        │ │   │ │   ├─┬ generate-object-property@1.2.0
        │ │   │ │   │ └── is-property@1.0.2
        │ │   │ │   ├── jsonpointer@4.0.0
        │ │   │ │   └── xtend@4.0.1
        │ │   │ ├─┬ hawk@3.1.3
        │ │   │ │ ├── boom@2.10.1
        │ │   │ │ ├── cryptiles@2.0.5
        │ │   │ │ ├── hoek@2.16.3
        │ │   │ │ └── sntp@1.0.9
        │ │   │ ├─┬ http-signature@1.1.1
        │ │   │ │ ├── assert-plus@0.2.0
        │ │   │ │ ├─┬ jsprim@1.3.1
        │ │   │ │ │ ├── extsprintf@1.0.2
        │ │   │ │ │ ├── json-schema@0.2.3
        │ │   │ │ │ └── verror@1.3.6
        │ │   │ │ └─┬ sshpk@1.10.1
        │ │   │ │   ├── asn1@0.2.3
        │ │   │ │   ├── assert-plus@1.0.0
        │ │   │ │   ├── bcrypt-pbkdf@1.0.0
        │ │   │ │   ├─┬ dashdash@1.14.0
        │ │   │ │   │ └── assert-plus@1.0.0
        │ │   │ │   ├── ecc-jsbn@0.1.1
        │ │   │ │   ├─┬ getpass@0.1.6
        │ │   │ │   │ └── assert-plus@1.0.0
        │ │   │ │   ├── jodid25519@1.0.2
        │ │   │ │   ├── jsbn@0.1.0
        │ │   │ │   └── tweetnacl@0.14.3
        │ │   │ ├── is-typedarray@1.0.0
        │ │   │ ├── isstream@0.1.2
        │ │   │ ├── json-stringify-safe@5.0.1
        │ │   │ ├── node-uuid@1.4.7
        │ │   │ ├── oauth-sign@0.8.2
        │ │   │ ├── qs@6.2.1
        │ │   │ ├── stringstream@0.0.5
        │ │   │ └── tunnel-agent@0.4.3
        │ │   ├── sax@1.2.1
        │ │   ├── symbol-tree@3.1.4
        │ │   ├── tough-cookie@2.3.1
        │ │   ├── webidl-conversions@2.0.1
        │ │   ├─┬ whatwg-url-compat@0.6.5
        │ │   │ └── tr46@0.0.3
        │ │   └── xml-name-validator@2.0.1
        │ ├─┬ hexo-cli@1.0.2
        │ │ └── minimist@1.2.0
        │ ├── hexo-front-matter@0.2.3
        │ ├─┬ hexo-fs@0.1.6
        │ │ ├─┬ chokidar@1.6.0
        │ │ │ ├─┬ anymatch@1.3.0
        │ │ │ │ ├── arrify@1.0.1
        │ │ │ │ └─┬ micromatch@2.3.11
        │ │ │ │   ├─┬ arr-diff@2.0.0
        │ │ │ │   │ └── arr-flatten@1.0.1
        │ │ │ │   ├── array-unique@0.2.1
        │ │ │ │   ├─┬ braces@1.8.5
        │ │ │ │   │ ├─┬ expand-range@1.8.2
        │ │ │ │   │ │ └─┬ fill-range@2.2.3
        │ │ │ │   │ │   ├── is-number@2.1.0
        │ │ │ │   │ │   ├─┬ isobject@2.1.0
        │ │ │ │   │ │   │ └── isarray@1.0.0
        │ │ │ │   │ │   ├── randomatic@1.1.5
        │ │ │ │   │ │   └── repeat-string@1.5.4
        │ │ │ │   │ ├── preserve@0.2.0
        │ │ │ │   │ └── repeat-element@1.1.2
        │ │ │ │   ├─┬ expand-brackets@0.1.5
        │ │ │ │   │ └── is-posix-bracket@0.1.1
        │ │ │ │   ├── extglob@0.3.2
        │ │ │ │   ├── filename-regex@2.0.0
        │ │ │ │   ├─┬ kind-of@3.0.4
        │ │ │ │   │ └── is-buffer@1.1.4
        │ │ │ │   ├── normalize-path@2.0.1
        │ │ │ │   ├─┬ object.omit@2.0.0
        │ │ │ │   │ ├─┬ for-own@0.1.4
        │ │ │ │   │ │ └── for-in@0.1.6
        │ │ │ │   │ └── is-extendable@0.1.1
        │ │ │ │   ├─┬ parse-glob@3.0.4
        │ │ │ │   │ ├── glob-base@0.3.0
        │ │ │ │   │ └── is-dotfile@1.0.2
        │ │ │ │   └─┬ regex-cache@0.4.3
        │ │ │ │     ├── is-equal-shallow@0.1.3
        │ │ │ │     └── is-primitive@2.0.0
        │ │ │ ├── async-each@1.0.1
        │ │ │ ├── UNMET OPTIONAL DEPENDENCY fsevents@^1.0.0
        │ │ │ ├── glob-parent@2.0.0
        │ │ │ ├── inherits@2.0.3
        │ │ │ ├─┬ is-binary-path@1.0.1
        │ │ │ │ └── binary-extensions@1.7.0
        │ │ │ ├─┬ is-glob@2.0.1
        │ │ │ │ └── is-extglob@1.0.0
        │ │ │ ├── path-is-absolute@1.0.1
        │ │ │ └─┬ readdirp@2.1.0
        │ │ │   ├─┬ readable-stream@2.1.5
        │ │ │   │ ├── buffer-shims@1.0.0
        │ │ │   │ ├── isarray@1.0.0
        │ │ │   │ ├── process-nextick-args@1.0.7
        │ │ │   │ └── util-deprecate@1.0.2
        │ │ │   └── set-immediate-shim@1.0.1
        │ │ └── graceful-fs@4.1.9
        │ ├─┬ hexo-i18n@0.2.1
        │ │ └── sprintf-js@1.0.3
        │ ├─┬ hexo-log@0.1.2
        │ │ └─┬ bunyan@1.8.1
        │ │   ├─┬ dtrace-provider@0.6.0
        │ │   │ └── nan@2.4.0
        │ │   ├─┬ mv@2.1.1
        │ │   │ ├── ncp@2.0.0
        │ │   │ └─┬ rimraf@2.4.5
        │ │   │   └── glob@6.0.4
        │ │   └── safe-json-stringify@1.0.3
        │ ├─┬ hexo-util@0.6.0
        │ │ ├─┬ camel-case@3.0.0
        │ │ │ ├─┬ no-case@2.3.0
        │ │ │ │ └── lower-case@1.1.3
        │ │ │ └── upper-case@1.1.3
        │ │ ├─┬ cross-spawn@4.0.2
        │ │ │ ├─┬ lru-cache@4.0.1
        │ │ │ │ ├── pseudomap@1.0.2
        │ │ │ │ └── yallist@2.0.0
        │ │ │ └─┬ which@1.2.11
        │ │ │   └── isexe@1.1.2
        │ │ ├── highlight.js@9.7.0
        │ │ ├── html-entities@1.2.0
        │ │ └── striptags@2.1.1
        │ ├─┬ js-yaml@3.6.1
        │ │ ├── argparse@1.0.9
        │ │ └── esprima@2.7.3
        │ ├── lodash@4.16.4
        │ ├─┬ minimatch@3.0.3
        │ │ └─┬ brace-expansion@1.1.6
        │ │   ├── balanced-match@0.4.2
        │ │   └── concat-map@0.0.1
        │ ├── moment@2.13.0
        │ ├── moment-timezone@0.5.6
        │ ├─┬ nunjucks@2.5.2
        │ │ ├── asap@2.0.5
        │ │ └─┬ yargs@3.32.0
        │ │   ├── camelcase@2.1.1
        │ │   ├─┬ cliui@3.2.0
        │ │   │ └── wrap-ansi@2.0.0
        │ │   ├── decamelize@1.2.0
        │ │   ├─┬ os-locale@1.4.0
        │ │   │ └─┬ lcid@1.0.0
        │ │   │   └── invert-kv@1.0.0
        │ │   ├─┬ string-width@1.0.2
        │ │   │ ├─┬ code-point-at@1.0.1
        │ │   │ │ └── number-is-nan@1.0.1
        │ │   │ └── is-fullwidth-code-point@1.0.0
        │ │   ├── window-size@0.1.4
        │ │   └── y18n@3.2.1
        │ ├── pretty-hrtime@1.0.2
        │ ├─┬ strip-indent@1.0.1
        │ │ └── get-stdin@4.0.1
        │ ├─┬ swig@1.4.2
        │ │ ├─┬ optimist@0.6.1
        │ │ │ ├── minimist@0.0.10
        │ │ │ └── wordwrap@0.0.3
        │ │ └─┬ uglify-js@2.4.24
        │ │   ├── async@0.2.10
        │ │   ├── source-map@0.1.34
        │ │   ├── uglify-to-browserify@1.0.2
        │ │   └─┬ yargs@3.5.4
        │ │     ├── camelcase@1.2.1
        │ │     ├── window-size@0.1.0
        │ │     └── wordwrap@0.0.2
        │ ├─┬ swig-extras@0.0.1
        │ │ └─┬ markdown@0.5.0
        │ │   └── nopt@2.1.2
        │ ├── text-table@0.2.0
        │ ├─┬ tildify@1.2.0
        │ │ └── os-homedir@1.0.2
        │ ├── titlecase@1.1.2
        │ └─┬ warehouse@2.2.0
        │   ├─┬ cuid@1.3.8
        │   │ ├── browser-fingerprint@0.0.1
        │   │ ├── core-js@1.2.7
        │   │ └── node-fingerprint@0.0.2
        │   ├─┬ is-plain-object@2.0.1
        │   │ └── isobject@1.0.2
        │   └─┬ JSONStream@1.2.1
        │     ├── jsonparse@1.2.0
        │     └── through@2.3.8
        ├── hexo-deployer-git@0.2.0
        ├─┬ hexo-generator-archive@0.1.4
        │ ├─┬ hexo-pagination@0.0.2
        │ │ └── utils-merge@1.0.0
        │ └── object-assign@2.1.1
        ├─┬ hexo-generator-category@0.1.3
        │ └── object-assign@2.1.1
        ├── hexo-generator-feed@1.2.0 extraneous
        ├─┬ hexo-generator-index@0.2.0
        │ └── object-assign@4.1.0
        ├── hexo-generator-search@1.0.2 extraneous
        ├── hexo-generator-tag@0.2.0
        ├─┬ hexo-renderer-ejs@0.2.0
        │ └── ejs@1.0.0
        ├─┬ hexo-renderer-marked@0.2.11
        │ └── marked@0.3.6
        ├─┬ hexo-renderer-stylus@0.3.1
        │ ├─┬ nib@1.1.2
        │ │ └─┬ stylus@0.54.5
        │ │   ├─┬ glob@7.0.6
        │ │   │ ├── fs.realpath@1.0.0
        │ │   │ ├─┬ inflight@1.0.6
        │ │   │ │ └── wrappy@1.0.2
        │ │   │ └── once@1.4.0
        │ │   ├── sax@0.5.8
        │ │   └── source-map@0.1.43
        │ └─┬ stylus@0.53.0
        │   ├── css-parse@1.7.0
        │   ├─┬ debug@2.2.0
        │   │ └── ms@0.7.1
        │   ├─┬ glob@3.2.11
        │   │ └─┬ minimatch@0.3.0
        │   │   ├── lru-cache@2.7.3
        │   │   └── sigmund@1.0.1
        │   ├─┬ mkdirp@0.5.1
        │   │ └── minimist@0.0.8
        │   ├── sax@0.5.8
        │   └─┬ source-map@0.1.43
        │     └── amdefine@1.0.0
        └─┬ hexo-server@0.2.0
          ├─┬ compression@1.6.2
          │ ├─┬ accepts@1.3.3
          │ │ ├── mime-types@2.1.12
          │ │ └── negotiator@0.6.1
          │ ├── bytes@2.3.0
          │ ├─┬ compressible@2.0.8
          │ │ └── mime-db@1.24.0
          │ ├── on-headers@1.0.1
          │ └── vary@1.1.0
          ├─┬ connect@3.5.0
          │ ├─┬ finalhandler@0.5.0
          │ │ ├── statuses@1.3.0
          │ │ └── unpipe@1.0.0
          │ └── parseurl@1.3.1
          ├── mime@1.3.4
          ├─┬ morgan@1.7.0
          │ ├── basic-auth@1.0.4
          │ ├── depd@1.1.0
          │ └─┬ on-finished@2.3.0
          │   └── ee-first@1.1.1
          ├─┬ opn@4.0.2
          │ └─┬ pinkie-promise@2.0.1
          │   └── pinkie@2.0.4
          └─┬ serve-static@1.11.1
            ├── encodeurl@1.0.1
            ├── escape-html@1.0.3
            └─┬ send@0.14.1
              ├── destroy@1.0.4
              ├── etag@1.7.0
              ├── fresh@0.3.0
              ├─┬ http-errors@1.5.0
              │ ├── inherits@2.0.1
              │ └── setprototypeof@1.0.1
              └── range-parser@1.2.0




[我的博客]: http://kidxueying.github.io
[Hexo]: http://hexo.io/
[hexo-theme-kidss]: https://github.com/kidxueying/hexo-theme-kidss
[hexo-theme-raytaylorism]: https://github.com/raytaylorism/hexo-theme-raytaylorism
