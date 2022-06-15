## 3.1.0
  - Refactor: switch to using the scheduler mixin [#22](https://github.com/logstash-plugins/logstash-output-cloudwatch/pull/22)

## 3.0.10
  - Deps: unpin rufus scheduler [#20](https://github.com/logstash-plugins/logstash-output-cloudwatch/pull/20)
  - Fix: an old undefined method error which would surface with load (as queue fills up) 

## 3.0.9
  - Fix: dropped usage of SHUTDOWN event deprecated since Logstash 5.0 [#18](https://github.com/logstash-plugins/logstash-output-cloudwatch/pull/18)

## 3.0.8
  - Docs: Set the default_codec doc attribute.

## 3.0.7
  - Update gemspec summary

## 3.0.6
  - Fix some documentation issues

## 3.0.4
  - Fix some remaining uses of the old event api. blocking the use of this plugin

## 3.0.3
  - Move some log messages from info to debug to avoid noise

## 3.0.2
  - Relax constraint on logstash-core-plugin-api to >= 1.60 <= 2.99

## 3.0.1
  - Republish all the gems under jruby.
## 3.0.0
  - Update the plugin to the version 2.0 of the plugin api, this change is required for Logstash 5.0 compatibility. See https://github.com/elastic/logstash/issues/5141
# 2.0.4
  - Depend on logstash-core-plugin-api instead of logstash-core, removing the need to mass update plugins on major releases of logstash
# 2.0.3
  - New dependency requirements for logstash-core for the 5.0 release
## 2.0.0
 - Plugins were updated to follow the new shutdown semantic, this mainly allows Logstash to instruct input plugins to terminate gracefully, 
   instead of using Thread.raise on the plugins' threads. Ref: https://github.com/elastic/logstash/pull/3895
 - Dependency on logstash-core update to 2.0

