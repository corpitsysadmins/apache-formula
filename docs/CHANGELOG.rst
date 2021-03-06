
Changelog
=========

`0.41.1 <https://github.com/saltstack-formulas/apache-formula/compare/v0.41.0...v0.41.1>`_ (2020-07-20)
-----------------------------------------------------------------------------------------------------------

Bug Fixes
^^^^^^^^^


* **server-status:** enable module in Debian family (\ `632802a <https://github.com/saltstack-formulas/apache-formula/commit/632802a5a946d2f05c40d9038d6f2ad596fafc58>`_\ )
* **server-status:** manage module in debian (\ `eafa419 <https://github.com/saltstack-formulas/apache-formula/commit/eafa4196d9495bc975c7e1e7036969bdaba1441d>`_\ )

Tests
^^^^^


* **default+modules:** add modules' tests suite (\ `b253625 <https://github.com/saltstack-formulas/apache-formula/commit/b25362535ae01dd140218b131a8e991d3a10cbe5>`_\ )

`0.41.0 <https://github.com/saltstack-formulas/apache-formula/compare/v0.40.0...v0.41.0>`_ (2020-07-16)
-----------------------------------------------------------------------------------------------------------

Features
^^^^^^^^


* **vhosts/standard:** add support for ScriptAlias in standard vhost (\ `b88b437 <https://github.com/saltstack-formulas/apache-formula/commit/b88b437308ff5d6bc504dabf9b69153db89f5b10>`_\ )

`0.40.0 <https://github.com/saltstack-formulas/apache-formula/compare/v0.39.5...v0.40.0>`_ (2020-07-16)
-----------------------------------------------------------------------------------------------------------

Features
^^^^^^^^


* **redhat/apache-2.x.config.jinja:** allow override of default_charset (\ `648f589 <https://github.com/saltstack-formulas/apache-formula/commit/648f589cc30684550c972d9cc4087e9e8b3fdc80>`_\ )

`0.39.5 <https://github.com/saltstack-formulas/apache-formula/compare/v0.39.4...v0.39.5>`_ (2020-06-21)
-----------------------------------------------------------------------------------------------------------

Bug Fixes
^^^^^^^^^


* **vhosts/cleanup:** check ``sites-enabled`` dir exists before listing it (\ `88373e3 <https://github.com/saltstack-formulas/apache-formula/commit/88373e38f55eab61cf1c4edc68324f3da48f7646>`_\ ), closes `#278 <https://github.com/saltstack-formulas/apache-formula/issues/278>`_

Continuous Integration
^^^^^^^^^^^^^^^^^^^^^^


* **gemfile.lock:** add to repo with updated ``Gemfile`` [skip ci] (\ `61b903e <https://github.com/saltstack-formulas/apache-formula/commit/61b903e7803eb80b50130834b90ca86d26b9d6c8>`_\ )
* **kitchen:** use ``saltimages`` Docker Hub where available [skip ci] (\ `6895fb9 <https://github.com/saltstack-formulas/apache-formula/commit/6895fb9764e9cebcbbff05763e367401d6cad959>`_\ )
* **kitchen+travis:** remove ``master-py2-arch-base-latest`` [skip ci] (\ `16bb1b0 <https://github.com/saltstack-formulas/apache-formula/commit/16bb1b06e351efdf9994676de38dec7b0ecd639d>`_\ )
* **travis:** add notifications => zulip [skip ci] (\ `2417a75 <https://github.com/saltstack-formulas/apache-formula/commit/2417a75fe218bd04c719f8eb2e2a7e402a20928e>`_\ )
* **workflows/commitlint:** add to repo [skip ci] (\ `2ce966d <https://github.com/saltstack-formulas/apache-formula/commit/2ce966d031e9044e8794dc93f605ce780fd99f12>`_\ )

`0.39.4 <https://github.com/saltstack-formulas/apache-formula/compare/v0.39.3...v0.39.4>`_ (2020-04-02)
-----------------------------------------------------------------------------------------------------------

Bug Fixes
^^^^^^^^^


* **mod_ssl:** update mod_ssl package variable to prevent clashes (\ `5591be2 <https://github.com/saltstack-formulas/apache-formula/commit/5591be26fddd234ebaed0e024969c45b6536ba82>`_\ )

`0.39.3 <https://github.com/saltstack-formulas/apache-formula/compare/v0.39.2...v0.39.3>`_ (2020-04-02)
-----------------------------------------------------------------------------------------------------------

Bug Fixes
^^^^^^^^^


* **debian:** generate remoteip conf before a2enconf (\ `1ed69f6 <https://github.com/saltstack-formulas/apache-formula/commit/1ed69f6c6fab0eb583949105e9e29e58b6ba32a3>`_\ )

Continuous Integration
^^^^^^^^^^^^^^^^^^^^^^


* **kitchen:** avoid using bootstrap for ``master`` instances [skip ci] (\ `275b5d5 <https://github.com/saltstack-formulas/apache-formula/commit/275b5d5e69fa79f1010852d65f0fcb65cadf735d>`_\ )
* **travis:** use ``major.minor`` for ``semantic-release`` version [skip ci] (\ `08cced2 <https://github.com/saltstack-formulas/apache-formula/commit/08cced29134ca47824e82ee6afa794233cdb5faa>`_\ )

`0.39.2 <https://github.com/saltstack-formulas/apache-formula/compare/v0.39.1...v0.39.2>`_ (2019-12-20)
-----------------------------------------------------------------------------------------------------------

Bug Fixes
^^^^^^^^^


* **redhat:** add user & group lookup to configs (\ `36ad2b2 <https://github.com/saltstack-formulas/apache-formula/commit/36ad2b24424936a4badeb7b4b2b26ee0d39e55f2>`_\ )

`0.39.1 <https://github.com/saltstack-formulas/apache-formula/compare/v0.39.0...v0.39.1>`_ (2019-12-20)
-----------------------------------------------------------------------------------------------------------

Bug Fixes
^^^^^^^^^


* **mod_mpm:** cast to int to avoid Jinja type mismatch error (\ `21045c7 <https://github.com/saltstack-formulas/apache-formula/commit/21045c7a7b46d639c2d81c5793ad6e6d9d34b66b>`_\ )

`0.39.0 <https://github.com/saltstack-formulas/apache-formula/compare/v0.38.2...v0.39.0>`_ (2019-12-20)
-----------------------------------------------------------------------------------------------------------

Continuous Integration
^^^^^^^^^^^^^^^^^^^^^^


* **gemfile:** restrict ``train`` gem version until upstream fix [skip ci] (\ `13be6f9 <https://github.com/saltstack-formulas/apache-formula/commit/13be6f9fac5aae55c48f74c784335c61d7fbaaf2>`_\ )
* **travis:** apply changes from build config validation [skip ci] (\ `0aac479 <https://github.com/saltstack-formulas/apache-formula/commit/0aac479c253f95b7fdcb1505476638c2d703bc77>`_\ )
* **travis:** opt-in to ``dpl v2`` to complete build config validation (\ `19e90ea <https://github.com/saltstack-formulas/apache-formula/commit/19e90ea2d6ef91118ebf59817ef4c91ad876af54>`_\ )
* **travis:** quote pathspecs used with ``git ls-files`` [skip ci] (\ `6608ddf <https://github.com/saltstack-formulas/apache-formula/commit/6608ddf8c5a361b93e6a44658ab1e306953566bf>`_\ )
* **travis:** run ``shellcheck`` during lint job [skip ci] (\ `2ff6b2f <https://github.com/saltstack-formulas/apache-formula/commit/2ff6b2f17e1fd48b5f0a4156c2dbd90f07f27025>`_\ )
* **travis:** use build config validation (beta) [skip ci] (\ `73160b2 <https://github.com/saltstack-formulas/apache-formula/commit/73160b249124df6bbd36b113df71724c019a118f>`_\ )

Features
^^^^^^^^


* **server-status:** allow remote servers to reach server-status page (\ `a3c0022 <https://github.com/saltstack-formulas/apache-formula/commit/a3c0022d7988eee0ec43d939bced91dee9fec0e1>`_\ )

`0.38.2 <https://github.com/saltstack-formulas/apache-formula/compare/v0.38.1...v0.38.2>`_ (2019-11-07)
-----------------------------------------------------------------------------------------------------------

Bug Fixes
^^^^^^^^^


* **apache/modules.sls:** fix duplicated ID (\ `57afd71 <https://github.com/saltstack-formulas/apache-formula/commit/57afd71627eb554138c8d5ec9cc790d899ed80ff>`_\ )

`0.38.1 <https://github.com/saltstack-formulas/apache-formula/compare/v0.38.0...v0.38.1>`_ (2019-11-05)
-----------------------------------------------------------------------------------------------------------

Bug Fixes
^^^^^^^^^


* **mod_perl2.sls:** fix a2enmod perl2 error (\ `fba8d21 <https://github.com/saltstack-formulas/apache-formula/commit/fba8d217944c8b5a0abf19cdbae7d41d1ec5bf2e>`_\ )
* **release.config.js:** use full commit hash in commit link [skip ci] (\ `dc5593c <https://github.com/saltstack-formulas/apache-formula/commit/dc5593cfdf775e065ea5f680f2ed2b6b7c80d8ed>`_\ )

Continuous Integration
^^^^^^^^^^^^^^^^^^^^^^


* **kitchen:** use ``debian-10-master-py3`` instead of ``develop`` [skip ci] (\ `09d82a5 <https://github.com/saltstack-formulas/apache-formula/commit/09d82a581caa09298d3d99ded215c5e45c5b619f>`_\ )
* **kitchen:** use ``develop`` image until ``master`` is ready (\ ``amazonlinux``\ ) [skip ci] (\ `d0bf6f3 <https://github.com/saltstack-formulas/apache-formula/commit/d0bf6f37969a9a97a6e368278e0f9eb40431f2f1>`_\ )
* **kitchen+travis:** upgrade matrix after ``2019.2.2`` release [skip ci] (\ `fc0f869 <https://github.com/saltstack-formulas/apache-formula/commit/fc0f869b78ef56369e1cfb6ff3d62179f703efa0>`_\ )
* **travis:** update ``salt-lint`` config for ``v0.0.10`` [skip ci] (\ `2622d48 <https://github.com/saltstack-formulas/apache-formula/commit/2622d48b4ccb01cd70555d46759d79d82d1db7bf>`_\ )

Performance Improvements
^^^^^^^^^^^^^^^^^^^^^^^^


* **travis:** improve ``salt-lint`` invocation [skip ci] (\ `bf75770 <https://github.com/saltstack-formulas/apache-formula/commit/bf7577022040a155de8b3ab4f557dd05484d278c>`_\ )

`0.38.0 <https://github.com/saltstack-formulas/apache-formula/compare/v0.37.4...v0.38.0>`_ (2019-10-20)
-----------------------------------------------------------------------------------------------------------

Bug Fixes
^^^^^^^^^


* **apache-2.2.config.jinja:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/f4045ef>`_\ )
* **apache-2.4.config.jinja:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/e2c1c2e>`_\ )
* **flags.sls:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/a146c59>`_\ )
* **init.sls:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/8465eb4>`_\ )
* **map.jinja:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/d011324>`_\ )
* **mod_geoip.sls:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/e55ef9b>`_\ )
* **modsecurity.conf.jinja:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/2a79d05>`_\ )
* **modules.sls:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/55d11f8>`_\ )
* **server_status.sls:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/da9a592>`_\ )
* **uninstall.sls:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/ed7dc7b>`_\ )
* **vhosts/cleanup.sls:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/b0bbd0b>`_\ )
* **vhosts/minimal.tmpl:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/146dc67>`_\ )
* **vhosts/proxy.tmpl:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/e7c9fbb>`_\ )
* **vhosts/redirect.tmpl:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/0a41b19>`_\ )
* **vhosts/standard.tmpl:** fix ``salt-lint`` errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/1bad58d>`_\ )
* **yamllint:** fix all errors (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/97f6ead>`_\ )

Documentation
^^^^^^^^^^^^^


* **formula:** use standard structure (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/701929d>`_\ )
* **readme:** move to ``docs/`` directory and modify accordingly (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/6933f0e>`_\ )

Features
^^^^^^^^


* **semantic-release:** implement for this formula (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/34d1f7c>`_\ )

Tests
^^^^^


* **mod_security_spec:** convert from Serverspec to InSpec (\ ` <https://github.com/saltstack-formulas/apache-formula/commit/68b971b>`_\ )
