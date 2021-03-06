Change log
==========


1.2.0
-----
* Bump version to 1.2.0 [2016-06-18 06:37:07 +0200]
* Add test for server disconnect and tcp error [2016-06-18 06:27:51 +0200]
* Fixes typo: Set active once after executing prepared statement [2016-06-18 06:27:43 +0200]
* Stop the gen_server when mysql server closes connection [2016-06-11 16:11:06 +0200]
* Properly handling empty passwords [2016-02-19 16:41:09 -0800]
* this change required for the elixir/exrm to package this as a dependency. [2016-01-05 12:40:41 -0600]

1.1.1
-----
* Bumb version 1.1.1 [2015-09-13 12:09:33 +0200]
* Skip lock wait timeout test when setting the timeout is not possible [2015-09-13 11:56:57 +0200]
* Don't check the multi capabilities from the server; fixes #31 [2015-09-13 11:55:46 +0200]
* Update CHANGELOG.md [2015-08-31 16:39:43 +0200]

1.1.0
-----
* Bump version 1.1.0 and update README [2015-08-31 14:51:56 +0200]
* add decode_binary clause for floats with value 0.0 [2015-08-30 20:45:47 +0200]
* Edit docs and tests for unicode chardata as input [2015-08-27 16:17:09 +0200]
* add encoding declaration [2015-08-25 12:13:57 +0200]
* add unicode encoding to mysql:encode, update docs and add test [2015-08-25 11:45:06 +0200]
* Support for strings as prepared statement parameters [2015-08-19 12:19:22 +0200]
* Update CHANGELOG.md [2015-05-25 16:26:02 +0200]

1.0.0
-----
* Bump version to 1.0.0 [2015-05-25 16:24:28 +0200]
* Simplify parsing server version [2015-05-25 16:11:15 +0200]
* Use erlang.mk for tests and coverage report [2015-05-25 15:13:29 +0200]
* Update erlang.mk [2015-05-25 15:10:56 +0200]
* Add CHANGELOG.md and a make target to build it. [2015-04-10 14:20:01 +0200]
* Add test case for initial queries returning results that are discarded. [2015-04-09 18:35:04 +0200]

0.9.0
-----
* Bump version. [2015-04-09 18:08:58 +0200]
* Allow empty auth plugin name in handshake. [2015-04-09 18:01:41 +0200]
* Implement multiple statements and multiple result sets. [2015-04-02 13:56:09 +0200]
* Add applications entry to .app.src file needed for relx. [2015-04-02 13:53:38 +0200]
* add compartibility with mysql versions like 5.5.33a [2015-04-01 19:52:22 +0200]
* Timeouts on fetching warnings and fetching results of cancelled queries. [2015-03-10 12:19:40 +0100]
* Version update in deps examples [2015-02-25 13:52:09 +0100]

0.8.1
-----
* Global replace in mysql:encode/2 fixes #15 [2015-01-15 11:50:18 +0100]
* DEPS example [2015-01-13 00:00:37 +0100]
* Adds link to 'MySQL/OTP + Poolboy' [2015-01-09 17:26:35 +0100]

0.8.0
-----
* Bump version [2015-01-09 14:56:55 +0100]
* Option for extra TCP options [2015-01-07 12:04:09 +0100]
* README: Usage as dependency [2015-01-07 12:02:58 +0100]
* Fix warning for unused variable [2015-01-07 12:01:43 +0100]
* Execute qeries and prepared statements on connect [2015-01-05 15:47:30 +0100]
* Small change in usage example [2014-12-29 16:39:11 +0100]
* mysql:encode/2 with tests [2014-12-29 15:00:50 +0100]
* Fixes dialyzer warnings + removes unused stuff [2014-12-28 13:16:37 +0100]

0.7.1
-----
* Minor typos in docs and tests [2014-12-19 23:15:42 +0100]

0.7.0
-----
* Bump version 0.7.0 [2014-12-19 21:31:39 +0100]
* More tests fixes #2 [2014-12-19 21:29:45 +0100]
* Keep alive (ping) [2014-12-19 17:14:03 +0100]
* Simplify error handling for implicit commit [2014-12-19 12:22:10 +0100]
* Named EUnit test cases [2014-12-18 20:27:49 +0100]
* Test that warnings are logged [2014-12-18 20:15:08 +0100]
* Restartable transactions and implicit commits and rollbacks, fixes #7 [2014-12-18 19:57:19 +0100]
* Typo in edoc [2014-12-18 19:55:04 +0100]
* Disable logging of most warnings in tests [2014-12-17 02:20:01 +0100]
* Minor change + more time to timeout sensitive test [2014-12-17 02:07:04 +0100]
* Log warnings [2014-12-17 01:00:12 +0100]

0.6.0
-----
* Bump version 0.6.0 (nested transactions) [2014-12-16 18:46:13 +0100]
* Nested transactions [2014-12-16 18:45:26 +0100]

0.5.1
-----
* Patch version [2014-12-15 23:05:49 +0100]
* More test cases; coverage to 96% [2014-12-15 23:05:30 +0100]
* Compatibility with erlang.mk [2014-12-15 22:21:28 +0100]
* Adds missing test helper module [2014-12-15 18:38:51 +0100]

0.5.0
-----
* Bump version 0.5.0 [2014-12-13 23:16:28 +0100]
* Graceful timeout handling using KILL QUERY [2014-12-13 23:03:43 +0100]
* Avoid dict:is_empty/1 for compat with old OTP versions [2014-12-10 23:13:11 +0100]
* Add parametrized queries to README [2014-12-10 23:06:33 +0100]
* Parametrized queries using cached prep. stmts [2014-12-10 22:59:54 +0100]
* docs and specs [2014-12-10 22:39:41 +0100]
* Fixes test for R16B by avoiding sys:get_state/1 [2014-12-09 13:30:00 +0100]
* Implements selecting db in the connection phase [2014-12-09 10:47:15 +0100]
* Merges mysql_connection with mysql [2014-12-09 10:08:36 +0100]

0.4.0
-----
* Bump version 0.4.0: changed value representation for some types [2014-12-08 02:00:30 +0100]
* DECIMAL(P,S) as int/float/binary depending on P and S [2014-12-08 01:41:41 +0100]
* Implements BIT(N) <--> bitstring() of length N [2014-12-07 19:53:30 +0100]
* Fixes decode TINYINT as signed in binary protocol [2014-12-07 19:12:31 +0100]
* Refactoring [2014-12-07 19:11:11 +0100]

0.3.0
-----
* Bump version 0.3.0 [2014-12-04 00:40:23 +0100]
* Add option {name, ServerName} and mysql_connection:start_link/1 [2014-12-04 00:36:25 +0100]
* Send goodbye when terminating [2014-12-03 10:49:06 +0100]
* Minor text changes [2014-12-03 01:13:41 +0100]
* Named prepared statements + unprepare/2 + {error, not_prepared} for execute/3 [2014-12-03 01:11:35 +0100]
* Makefile rules for gh-pages [2014-12-01 22:46:57 +0100]
* Documentation [2014-12-01 02:06:34 +0100]

0.2.0
-----
* Add autocommit/1 [2014-11-30 17:00:50 +0100]
* in_transaction/1 (related to #7) [2014-11-30 16:42:34 +0100]
* Edoc and spec [2014-11-30 15:46:15 +0100]
* Implements simple mnesia style transactions (#7) [2014-11-29 22:51:42 +0100]
* Changed transaction example [2014-11-29 12:56:57 +0100]
* Notes about LGPL + logo fix [2014-11-28 22:17:51 +0100]
* Change license to LGPL [2014-11-28 21:05:48 +0100]
* Set up Travis build [2014-11-27 03:03:34 +0100]
* Typo in travis file [2014-11-27 02:03:58 +0100]
* Adds travis ci file [2014-11-27 02:00:56 +0100]
* Adds note on license compatibility issues [2014-11-25 19:06:28 +0100]

0.1.1
-----
* Patch version [2014-11-27 01:25:41 +0100]
* Error message formatting [2014-11-27 01:24:00 +0100]
* Fixes handshake for servers without CLIENT_PLUGIN_AUTH [2014-11-27 01:23:33 +0100]
* EDoc overview page and custom CSS [2014-11-25 02:07:53 +0100]

0.1.0
-----
* Bump version [2014-11-24 22:46:34 +0100]
* Negative TIME, microseconds in TIME and DATETIME, new TIME representation [2014-11-24 22:45:24 +0100]
* How to run the tests [2014-11-23 13:04:21 +0100]
* Renames some functions [2014-11-20 19:33:44 +0100]
* Update README.md [2014-11-18 10:26:44 +0100]
* Update README.md [2014-11-18 10:09:43 +0100]
* Float rounding; see #4 [2014-11-18 09:28:46 +0100]
* Binary protocol [2014-11-15 19:25:27 +0100]
* Adds a failing test for float (precicion loss) [2014-11-05 09:30:24 +0100]
* Refactoring [2014-11-05 09:12:18 +0100]
* Prepared statements without params (bin protocol) [2014-11-04 22:03:09 +0100]
* Add licence information [2014-11-04 18:01:53 +0100]
* Test for password hash [2014-11-03 00:14:41 +0100]
* Prepared statements partially + various fixes [2014-11-02 23:52:02 +0100]
* Use the timeout option in all TCP recv calls [2014-11-02 22:47:26 +0100]
* Comments and errors [2014-11-02 22:46:40 +0100]
* Implement plain queries and the text protocol [2014-11-02 16:19:41 +0100]
* Update README.md [2014-10-28 22:25:12 +0100]
* Implements handshake and basic protocol [2014-10-28 16:44:14 +0100]
* Initial commit [2014-10-28 16:38:08 +0100]
