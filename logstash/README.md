To debug Grok patterns, use this [online](http://grokdebug.herokuapp.com/) debugger. Another [one](http://grokconstructor.appspot.com).

```sh
linux@linux:~/monitoring-tools/logstash$ sudo logstash -f logstash-java.conf
```

The output of successfull logs which match looks like the following:

```ruby
{
         "mylog" => "Sending artifact Ω25ΥΩΗΒ-0ΡΩ (61796 bytes) to storage\r",
          "path" => "/home/linux/projects/log-analysis/2016_12_09.stderrout.log.105016910",
    "@timestamp" => 2016-12-12T17:21:09.233Z,
          "sbob" => "2016-12-09 10:49:37,910 INFO  DecisionMediaServiceImpl - Sending artifact Ω25ΥΩΗΒ-0ΡΩ (61796 bytes) to storage\r",
      "loglevel" => "INFO",
      "@version" => "1",
          "host" => "lubuntus",
       "message" => "2016-12-09 10:49:37,910 INFO  DecisionMediaServiceImpl - Sending artifact Ω25ΥΩΗΒ-0ΡΩ (61796 bytes) to storage\r",
         "class" => "DecisionMediaServiceImpl",
          "tags" => []
}
{
         "mylog" => "The artifact Ω25ΥΩΗΒ-0ΡΩ has been stored\r",
          "path" => "/home/linux/projects/log-analysis/2016_12_09.stderrout.log.105016910",
    "@timestamp" => 2016-12-12T17:21:09.233Z,
          "sbob" => "2016-12-09 10:49:38,144 INFO  DecisionMediaServiceImpl - The artifact Ω25ΥΩΗΒ-0ΡΩ has been stored\r",
      "loglevel" => "INFO",
      "@version" => "1",
          "host" => "lubuntus",
       "message" => "2016-12-09 10:49:38,144 INFO  DecisionMediaServiceImpl - The artifact Ω25ΥΩΗΒ-0ΡΩ has been stored\r",
         "class" => "DecisionMediaServiceImpl",
          "tags" => []
}
{
         "mylog" => "User 6191_admin is logged in, Lumi-Token-Response value: 6191_admin:1481280581832:6d5488290219d5d40377f7c52d8877db\r",
          "path" => "/home/linux/projects/log-analysis/2016_12_09.stderrout.log.105016910",
    "@timestamp" => 2016-12-12T17:21:09.234Z,
          "sbob" => "2016-12-09 10:49:41,832 INFO  LumiTokenAuthenticationFilter - User 6191_admin is logged in, Lumi-Token-Response value: 6191_admin:1481280581832:6d5488290219d5d40377f7c52d8877db\r",
      "loglevel" => "INFO",
      "@version" => "1",
          "host" => "lubuntus",
       "message" => "2016-12-09 10:49:41,832 INFO  LumiTokenAuthenticationFilter - User 6191_admin is logged in, Lumi-Token-Response value: 6191_admin:1481280581832:6d5488290219d5d40377f7c52d8877db\r",
         "class" => "LumiTokenAuthenticationFilter",
          "tags" => []
}
{
         "mylog" => "User 5005_429 is logged in, Lumi-Token-Response value: 5005_429:1481280582051:a8ed8f438a6fac78808f8706be3155ac\r",
          "path" => "/home/linux/projects/log-analysis/2016_12_09.stderrout.log.105016910",
    "@timestamp" => 2016-12-12T17:21:09.234Z,
          "sbob" => "2016-12-09 10:49:42,051 INFO  LumiTokenAuthenticationFilter - User 5005_429 is logged in, Lumi-Token-Response value: 5005_429:1481280582051:a8ed8f438a6fac78808f8706be3155ac\r",
      "loglevel" => "INFO",
      "@version" => "1",
          "host" => "lubuntus",
       "message" => "2016-12-09 10:49:42,051 INFO  LumiTokenAuthenticationFilter - User 5005_429 is logged in, Lumi-Token-Response value: 5005_429:1481280582051:a8ed8f438a6fac78808f8706be3155ac\r",
         "class" => "LumiTokenAuthenticationFilter",
          "tags" => []
}

```