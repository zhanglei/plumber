# CHANGELOG

## HEAD (Unreleased)
_(none)_

## 0.6.0 (2017-01-19)

* Fixed: fix for 0.6.0

## 0.6.0 (2017-01-19)

* Feature: 整体的使用方式变更，见README。

## 0.5.4 (2016-12-28)

* Feature: 去除了Plumber\Logger类，使用Monolog类替代。
* Feature: 使用Monolog\ErrorHandler捕获程序错误，并记录日志。
* Feature: 去除了`output_path`的配置，output输出的内容，合并到`log_path`所在文件。

## v0.5.3 (2016-07-26)

* Fixed: 当retry job时，向job body注入重试次数的变量名由`retry`改为`__retry`。

## v0.5.2 (2016-07-26)

* Fixed: 当抛出DeadlineSoonException时，休眠2秒后再reserve job。