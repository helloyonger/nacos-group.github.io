---
title: 提交需求模板
keywords: [pull request,模板]
description: 提交需求模板
---

# 提交需求模板

请不要只提交需求而不创建问题。

## What is the purpose of the change

XXXXX

## Brief changelog

XX

## Verifying this change

XXXX

Follow this checklist to help us incorporate your contribution quickly and easily:

* [ ] Make sure there is a Github issue filed for the change (usually before you start working on it). Trivial changes like typos do not require a Github issue. Your pull request should address just this issue, without pulling in other changes - one PR resolves one issue.
* [ ] Format the pull request title like `[ISSUE #123] Fix UnknownException when host config not exist`. Each commit in the pull request should have a meaningful subject line and body.
* [ ] Write a pull request description that is detailed enough to understand what the pull request does, how, and why.
* [ ] Write necessary unit-test to verify your logic correction, more mock a little better when cross module dependency exist. If the new feature or significant change is committed, please remember to add integration-test in [test module](https://github.com/apache/rocketmq/tree/master/test).
* [ ] Run `mvn -B clean apache-rat:check findbugs:findbugs` to make sure basic checks pass. Run `mvn clean install -DskipITs` to make sure unit-test pass. Run `mvn clean test-compile failsafe:integration-test`  to make sure integration-test pass.
* [ ] If this contribution is large, please file an [Apache Individual Contributor License Agreement](http://www.apache.org/licenses/#clas).