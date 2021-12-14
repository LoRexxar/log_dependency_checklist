# Log Dependencies with Log4j2 Checklist

All content of this project comes from https://maven.apache.org/ and is not responsible for the validity of the data.
The scan selected the first 400 components including log4j and log4j2 to obtain data.
If you have any questions, please PR.



本项目所有内容均来自于https://maven.apache.org/ ，不对数据有效性负责。
扫描选取了包含log4j和log4j2在内的前400个组件获取数据。
如果有任何问题欢迎PR.



**Newest log4j-core version**: the log4j-core version referenced in the latest version. Components lower than 2.15 need to manually update the log4j-core version, and the other can be directly upgraded and repaired.

指最新版本中引用的log4j-core版本，低于2.15的组件需要手动更新log4j-core版本，其余可直接升级修复。




# Vulnerable dependency



| dependency name                                        | Newest log4j-core version | usages | Vulnerable |
| ------------------------------------------------------------ | ------------------ | ------ | ---------- |
| org.apache.logging.log4j.log4j-slf4j-impl                    | 2.16.0             | 4829   | √         |
| org.apache.logging.log4j.log4j-jcl                           | 2.16.0             | 940    | √         |
| org.apache.logging.log4j.log4j-1.2-api                       | 2.16.0             | 846    | √         |
| org.springframework.boot.spring-boot-starter-log4j2          | 2.14.1             | 810    | √         |
| org.apache.logging.log4j.log4j-web                           | 2.16.0             | 716    | √         |
| org.apache.logging.log4j.log4j-slf4j18-impl                  | 2.16.0             | 471    | √         |
| org.apache.logging.log4j.log4j-jul                           | 2.16.0             | 329    | √         |
| org.apache.logging.log4j.log4j-iostreams                     | 2.16.0             | 60     | √         |
| org.ops4j.pax.logging.pax-logging-log4j2                     | 2.15.0             | 52     | √         |
| org.apache.logging.log4j.log4j                               | 2.16.0             | 43     | √         |
| com.amazonaws.aws-lambda-java-log4j2                         | 2.15.0             | 28     | √         |
| org.apache.logging.log4j.log4j-layout-template-json          | 2.16.0             | 25     | √         |
| org.apache.logging.log4j.adapters.slf4j-impl                 | 2.0-beta2          | 18     | √         |
| org.apache.logging.log4j.log4j-api-kotlin                    | 2.13.2             | 17     | √         |
| cd.connect.composites.java.connect-composite-log4j2          | [2.8.2]            | 16     | √         |
| org.apache.logging.log4j.adapters.log4j-jcl                  | 2.0-beta4          | 12     | √         |
| org.apache.ignite.ignite-log4j2                              | 2.11.0             | 12     | √         |
| org.apache.logging.log4j.adapters.log4j12-api                | 2.0-beta3          | 11     | √         |
| com.zensols.clj-append                                       | 2.7                | 11     | √         |
| org.apache.logging.log4j.log4j-bom                           | 2.16.0             | 10     | √         |
| com.gantzgulch.tools.gantzgulch-logging-log4j2               | 2.15.0             | 10     | √         |
| io.zipkin.brave.brave-context-log4j2                         | 2.14.0             | 9      | √         |
| com.epam.reportportal.logger-java-log4j                      | 2.15.0             | 8      | √         |
| io.sentry.sentry-log4j2                                      | 2.13.3             | 8      | √         |
| com.weicoder.log4j                                           | 2.14.0             | 7      | √         |
| io.apiman.apiman-common-logging-log4j2                       | 2.15.0             | 7      | √         |
| org.apache.logging.log4j.log4j-nosql                         | 2.9.1              | 6      | √         |
| org.openscience.cdk.cdk-log4j                                | 2.13.3             | 5      | √         |
| org.appenders.log4j.log4j2-elasticsearch-core                | 2.13.3             | 5      | √         |
| co.elastic.logging.log4j2-ecs-layout                         | 2.14.0             | 5      | √         |
| de.heikoseeberger.akka-log4j                                 | 2.11.0             | 4      | √         |
| org.apache.logging.log4j.log4j-jpl                           | 2.16.0             | 4      | √         |
| org.apache.logging.log4j.adapters.log4j-slf4j-impl           | 2.0-beta4          | 4      | √         |
| org.apache.logging.log4j.slf4j-impl                          | 2.0-alpha2         | 4      | √         |
| io.scalecube.scalecube-benchmarks-log4j2                     | 2.11.1             | 4      | √         |
| com.vlkan.log4j2.log4j2-logstash-layout                      | 2.13.3             | 4      | √         |
| org.apache.logging.log4j.log4j-flume-ng                      | 2.16.0             | 3      | √         |
| org.apache.logging.log4j.log4j-audit-api                     | 2.10.0             | 3      | √         |
| de.hs-heilbronn.mi.log4j2-utils                              | 2.15.0             | 3      | √         |
| org.graylog2.log4j2.log4j2-gelf                              | 2.4.1              | 3      | √         |
| io.prometheus.simpleclient_log4j2                            | 2.1                | 3      | √         |
| net.mamoe.mirai-logging-log4j2                               | 2.15.0             | 3      | √         |
| io.dropwizard.metrics.metrics-log4j2                         | 2.14.1             | 3      | √         |
| io.servicetalk.servicetalk-log4j2-mdc-utils                  | 2.14.1             | 3      | √         |
| com.alibaba.log4j2-ttl-thread-context-map                    | 2.14.0             | 3      | √         |
| io.github.technologize.fluency-log4j-appender-core           | [2.11.0            | 2      | √         |
| org.apache.logging.log4j.log4j-catalog-jpa                   | 2.10.0             | 2      | √         |
| org.apache.logging.log4j.adapters.log4j-web                  | 2.0-beta4          | 2      | √         |
| org.apache.logging.log4j.log4j-catalog-git                   | 2.10.0             | 2      | √         |
| io.github.technologize.fluency-log4j-appender-core           | 2.11.0             | 2      | √         |
| com.expedia.www.haystack-log4j-metrics-appender              | 2.10.0             | 2      | √         |
| org.apache.logging.log4j.adapters.log4j-flume-ng             | 2.0-beta4          | 2      | √         |
| com.truthbean.log4j2-boot                                    | 2.14.1             | 2      | √         |
| com.sap.hcp.cf.logging.cf-java-logging-support-log4j2        | 2.15.0             | 2      | √         |
| org.gridgain.ignite-log4j2                                   | 2.13.3             | 2      | √         |
| com.carrotsearch.progresso.progresso-log4j2                  | 2.15.0             | 2      | √         |
| com.netflix.spectator.spectator-ext-log4j2                   | 2.15.0             | 2      | √         |
| com.getsentry.raven.raven-log4j2                             | 2.8.1              | 2      | √         |
| com.aliyun.openservices.aliyun-log-log4j2-appender           | 2.0.2              | 2      | √         |
| de.huxhorn.lilith.de.huxhorn.lilith.log4j2.converter         | 2.15.0             | 2      | √         |
| de.chandre.admin-tools.admin-tools-log4j2                    | 2.8.2              | 1      | √         |
| io.avaje.log4j                                               | 2.14.1             | 1      | √         |
| com.github.taucher2003.appenders.log4j                       | 2.14.1             | 1      | √         |
| io.sensefly.logging.log4j.log4j-cloudwatch-appender          | 2.9.1              | 1      | √         |
| io.pivotal.gemfire.geode-log4j                               | 2.12.1             | 1      | √         |
| org.apache.logging.log4j.log4j-spring-boot                   | 2.16.0             | 1      | √         |
| com.djdch.log4j.log4j-staticshutdown                         | 2.2                | 1      | √         |
| no.mnemonic.commons.logging-log4j                            | 2.15.0             | 1      | √         |
| com.flipkart.poseidon.log4j-access                           | 2.15.0             | 1      | √         |
| gradle.plugin.de.sebastianboegl.gradle.plugins.shadow-log4j-transformer | 2.+                | 1      | √         |
| org.apache.geode.geode-log4j                                 | 2.15.0             | 1      | √         |
| net.openhft.chronicle-logger-log4j-2                         | 2.14.1             | 1      | √         |
| org.apache.skywalking.apm-toolkit-log4j-2.x                  | 2.7                | 1      | √         |
| gradle.plugin.io.paulbaker.gradle-shaded-log4j-transformer   | 2.11.0             | 1      | √         |
| org.apache.logging.log4j.log4j-taglib                        | 2.16.0             | 1      | √         |
| org.apache.logging.log4j.log4j-appserver                     | 2.16.0             | 1      | √         |
| org.apache.logging.log4j.log4j12-api                         | 2.0-alpha2         | 1      | √         |
| org.apache.logging.log4j.adapters.log4j-1.2-api              | 2.0-beta4          | 1      | √         |
| science.aist.seshat.log4j2                                   | 2.14.1             | 1      | √         |
| funcool.log4j2-clojure                                       | 2.14.0             | 1      | √         |
| com.dinstone.loghub.loghub-log4j2                            | 2.5                | 1      | √         |
| com.netflix.karyon.karyon3-log4j2                            | 2.3                | 1      | √         |
| com.truthbean.logger.log4j2-adapter                          | 2.14.0             | 1      | √         |
| com.tersesystems.blacklite.blacklite-log4j2                  | 2.13.3             | 1      | √         |
| io.github.zqrferrari.logi-log-log4j2                         | 2.9.1              | 1      | √         |
| com.kumuluz.ee.logs.kumuluzee-logs-log4j2                    | 2.15.0             | 1      | √         |
| com.truthbean.logger-to-log4j2                               | 2.14.1             | 1      | √         |
| cn.q-game.akka-log4j2-logger                                 | 2.3                | 1      | √         |
| com.github.wolf480pl.jline-log4j2-appender                   | 2.0.2              | 1      | √         |
| org.bithon.agent.agent-plugin-logging-log4j2                 | 2.9.1              | 1      | √         |
| nz.net.osnz.composite.composite-logging-log4j2               | [2.14.0]           | 1      | √         |
| org.apache.samza.samza-log4j2                                | 2.12.0             | 1      | √         |
| com.kloudtek.mule.elogging.mule-elogging-log4j2              | 2.5                | 1      | √         |
| org.ops4j.pax.logging.pax-logging-sample-fragment-log4j2     | 2.15.0             | 1      | √         |
| com.plumelog.plumelog_log4j2                                 | 2.11.0             | 1      | √         |
| org.seppiko.glf.glf-log4j2                                   | 2.15.0             | 1      | √         |
| info.xiancloud.xian-log4j2                                   | 2.9.1              | 1      | √         |
| net.savantly.log4j2.extended-jsonlayout                      | 2.8.2              | 1      | √         |
| com.kangyonggan.app-log4j2                                   | 2.5                | 1      | √         |
| de.huxhorn.lilith.de.huxhorn.lilith.log4j2.decoder           | 2.15.0             | 1      | √         |
| com.truthbean.logger.log4j2-boot                             | 2.14.0             | 1      | √         |
| com.github.backtrace-labs.backtrace-log4j2.backtrace-log4j2  | 2.13.1             | 1      | √         |
| com.navercorp.pinpoint.pinpoint-log4j2-plugin-jdk8-it        | 2.13.3             | 1      | √         |
| io.github.m-moris.log4j2-azure-blob-appender                 | 2.13.2             | 1      | √         |
| com.github.ivanocortesini.log4j-2-elastic                    | 2.11.1             | 1      | √         |
| pw.krejci.calldepth-log4j2-plugin                            | 2.12.1             | 1      | √         |
| com.github.omkreddy.log4j2-kafka-appender                    | 2.3                | 1      | √         |
| net.inemar.utility.log4j2elastic                             | 2.1                | 1      | √         |
| org.appenders.log4j.log4j2-elasticsearch-hc                  | 2.13.3             | 1      | √         |
| org.appenders.log4j.log4j2-elasticsearch6-bulkprocessor      | 2.13.3             | 1      | √         |
| com.wuyushuo.wuyu-plugin-wlog4j                              | 2.3                | 1      | √         |
| com.gitlab.dmexe.logfmt-log4j2                               | 2.13.3             | 1      | √         |
| org.snf4j.snf4j-core-log4j2                                  | 2.11.2             | 1      | √         |
| com.vlkan.log4j2.log4j2-redis-appender-parent                | 2.14.1             | 1      | √         |
| com.atlassian.amps.amps-tomcat-log4j2                        | 2.11.0             | 1      | √         |
| com.dpxcn.support.log4j2.glc                                 | 2.3                | 1      | √         |
| de.agilecoders.elasticsearch.logger.log2es-log4j2            | 2.0-beta9          | 1      | √         |
| io.github.alexswilliams.logstash-log4j2-encoder              | 2.15.0             | 1      | √         |
| com.lightbend.lagom.lagom-log4j2                             | 2.12.1             | 1      | √         |
| org.bgee.log4jdbc-log4j2.log4jdbc-log4j2-jdbc3               | 2.0-beta4          | 1      | √         |
| arctype.log4j2-plugins-cache                                 | 2.11.0             | 1      | √         |
| org.appenders.log4j.log4j2-elasticsearch-jest                | 2.13.3             | 1      | √         |
| com.mastfrog.bunyan-log4j2-appender                          | 2.13.3             | 1      | √         |
| org.appenders.log4j.log4j2-elasticsearch5-bulkprocessor      | 2.13.3             | 1      | √         |
| com.firedrum.influxdb-log4j2                                 | 2.11.0             | 1      | √         |
| pl.tkowalcz.tjahzi.log4j2-appender                           | 2.13.3             | 1      | √         |
| simple.android.log4j2.log4j2-android                         | 2.3                | 1      | √         |
| io.confluent.confluent-log4j2-extensions                     | 2.13.2             | 1      | √         |
| com.sinnerschrader.metrics.metrics-log4j2                    | 2.0.2              | 1      | √         |
| io.airbrake.log4javabrake2                                   | 2.15.0             | 1      | √         |
| org.javastack.log4j2-jvmext                                  | 2.6.2              | 1      | √         |
| io.tracee.backend.tracee-log4j2                              | 2.0.2              | 1      | √         |
| org.javastack.log4j2-webext                                  | 2.6.2              | 1      | √         |
| data.be.sysa.log-sanitizer.log-sanitizer                     | 2.11.1             | 1      | √         |
| com.taobao.middleware.logger.log4j2.test                     | 2.8.2              | 1      | √         |
| io.github.c-a-services.log4j2-sftp-appender                  | 2.11.1             | 1      | √         |
| systems.microservice.log4j2-elasticsearch-appender           | 2.11.2             | 1      | √         |
| com.navercorp.pinpoint.pinpoint-log4j2-plugin-it             | 2.12.1             | 1      | √         |
| se.kth.infosys.log4j2.bunyan-layout                          | 2.6.2              | 1      | √         |
| com.github.swierkosz.log4j2-captor                           | 2.14.1             | 1      | √         |
| org.apache.pulsar.pulsar-log4j2-appender                     | 2.14.0             | 1      | √         |
| com.widdindustries.influx-log4j2-appender                    | 2.14.1             | 1      | √         |
| be.sysa.log-sanitizer.log-sanitizer-log4j2                   | 2.14.0             | 1      | √         |
| dev.galasa.dev.galasa.framework.log4j2.bridge                | 2.14.1             | 1      | √         |
| com.teragrep.jla_06                                          | 2.14.1             | 1      | √         |
| ai.h2o.h2o-logging-impl-log4j2                               | 2.14.1             | 1      | √         |
| com.google.flogger.flogger-log4j2-backend                    | 2.15.0             | 1      | √         |
| com.widdindustries.clojure.log4j2                            | 2.14.1             | 1      | √         |
| com.kloudtek.elogging.elogging-log4j2                        | 2.5                | 1      | √         |
| com.sumologic.plugins.log4j.sumologic-log4j2-appender        | 2.15.0             | 1      | √         |
| com.github.magrossi.log4j2-elasticsearch-appender            | 2.8.2              | 1      | √         |
| com.github.ivandzf.log4j2-custom-layout                      | 2.10.0             | 1      | √         |
| com.corp2world.c2w-java-client-log4j2                        | 2.1                | 1      | √         |
| io.opentelemetry.opentelemetry-extension-logging-log4j2-extensions | 2.13.3             | 1      | √         |
| com.dadapush.client.dadapush-log4j2-appender                 | 2.12.0             | 1      | √         |
| clj-log4j2.clj-log4j2                                        | 2.3                | 1      | √         |
| com.alipay.sofa.sofa-tracer-log4j2-test                      | 2.14.0             | 1      | √         |
| be.sysa.log-sanitizer.log-sanitizer                          | 2.14.0             | 1      | √         |
| com.kloudtek.mule-elogging.mule-elogging-log4j2              | 2.5                | 1      | √         |
| org.javastack.log4j2-simplejson                              | 2.8.2              | 1      | √         |
| com.carmatechnologies.commons.commons-testing-log4j2         | 2.1                | 1      | √         |
| me.drmaas.log4j2-logstash-layout                             | 2.11.1             | 1      | √         |
| io.opencensus.opencensus-contrib-log-correlation-log4j2      | 2.11.1             | 1      | √         |
| com.simple.android.log4j2-android                            | 2.3                | 1      | √         |
| com.aeontronix.log4j2.log4j2-enhanced-json-layout            | 2.5                | 1      | √         |
| com.kdgregory.logging.log4j2-aws-appenders                   | 2.8                | 1      | √         |
| com.techempower.gemini-log4j2                                | 2.13.3             | 1      | √         |
| com.github.rage28.log4j2-slack                               | 2.8.2              | 1      | √         |
| io.streamnative.pulsar-log4j2-appender                       | 2.10.0             | 1      | √         |
| com.vicrab.vicrab-log4j2                                     | 2.8.1              | 1      | √         |
| com.newrelic.logging.log4j2                                  | 2.13.3             | 1      | √         |
| koeln.niemeier.log4j2-json-layout                            | 2.7                | 1      | √         |
| io.bitsensor.plugins.bitsensor-log4j2                        | 2.2                | 1      | √         |
| opentoutatice-ecm.log4j2.opentoutatice-addon-log4j2-marketplace | 2.7                | 1      | √         |
| io.logz.log4j2.logzio-log4j2-appender                        | 2.15.0             | 1      | √         |
| com.github.stuxuhai.log4j2-kafka                             | 2.0.2              | 1      | √         |
| com.mariocairone.log4j2-masking-policy-parent                | 2.13.2             | 1      | √         |
| com.rollbar.rollbar-log4j2                                   | 2.11.0             | 1      | √         |
| com.github.edwgiz.maven-shade-plugin.log4j2-cachefile-transformer | 2.15.0             | 1      | √         |
| com.therealvan.appender-log4j2                               | 2.15.0             | 1      | √         |
| com.globo.graylog2.log4j2-gelf                               | 2.4.1              | 1      | √         |
| org.appenders.log4j.log4j2-elasticsearch2-bulkprocessor      | 2.13.3             | 1      | √         |
| org.crosslibs.extensible-json-layout                         | 2.9.0              | 1      | √         |
| io.enoa.enoa-log-log4j2                                      | 2.11.1             | 1      | √         |
| tech.raaf.logelastic                                         | 2.8.2              | 1      | √         |
| nz.net.osnz.composite.composite-log4j2                       | [2.12.1]           | 1      | √         |
| com.vlkan.log4j2.log4j2-logstash-layout-demo                 | 2.13.3             | 1      | √         |
| com.plumelog.plumelog-log4j2                                 | 2.11.0             | 1      | √         |
| br.com.ppm.ppm-logging                                       | 2.14.1             | 1      | √         |
| com.github.schnitker.logmanager.logmgr-log4j2                | 2.0.2              | 1      | √         |
| org.graylog2.log4j2.log4j2-gelf-opencast                     | 2.4.1              | 1      | √         |
| com.mariocairone.log4j2-prop-lookup                          | 2.13.0             | 1      | √         |
| com.nextdoor.rollbar.rollbar-log4j                           | 2.8.1              | 1      | √         |
| com.github.dekobon.log4j2-bunyan-layout                      | 2.14.1             | 1      | √         |
| com.github.akunzai.log4j2-sendgrid-appender                  | 2.15.0             | 1      | √         |
| com.m-creations.log4j2-native-syslog                         | 2.7                | 1      | √         |
| com.hedera.hashgraph.log4j2                                  | 2.13.1             | 1      | √         |
| com.coralogix.sdk.appenders.log4j2-appender                  | 2.3                | 1      | √         |
| com.qiniu.qiniu-logging-plugin-log4j2                        | 2.9.1              | 1      | √         |
| com.randomnoun.common.log4j-one-bridge                       | 2.14.0             | 1      | √         |
| org.bgee.log4jdbc-log4j2.log4jdbc-log4j2                     | 2.0-beta8          | 1      | √         |
| com.axibase.aggregation-log-filter-log4j2                    | 2.13.3             | 1      | √         |
| com.aeontronix.elogging.elogging-log4j2-json-layout          | 2.5                | 1      | √         |
| org.clojars.lukas.bleve-log4j-appender                       | 2.11.2             | 1      | √         |
| data.info.xiancloud.xian-log4j2                              | 2.9.1              | 1      | √         |
| io.github.githublaohu.log4j2-dependent                       | 2.13.3             | 1      | √         |
| com.gitlab.lema-suite.lema-provider-log4j2                   | 2.13.3             | 1      | √         |
| com.github.jimpil.flog                                       | 2.14.1             | 1      | √         |
| de.it-tw.log4j2-extras                                       | 2.11.1             | 1      | √         |
| com.iopipe.iopipe-logger-log4j2                              | 2.11.2             | 1      | √         |
| com.github.mlangc.zio-interop-log4j2                         | 2.13.3             | 1      | √         |
| com.mariocairone.log4j2-masking-policy                       | 2.13.2             | 1      | √         |
| com.vlkan.log4j2.log4j2-logstash-layout-parent               | 2.13.3             | 1      | √         |
| me.drmaas.log4j2-logstash-jsonevent-layout                   | 2.11.1             | 1      | √         |
| de.holisticon.util.tracee.backend.tracee-log4j2              | 2.0-rc1            | 1      | √         |
| com.github.dubasdey.log4j2-jsonevent-layout                  | 2.13.3             | 1      | √         |



# Non-vulnerable dependency



| dependency Name                                              | usages | vulnerable |
| ------------------------------------------------------------ | ------ | ---------- |
| log4j.log4j                                                  | 16606  | ×         |
| org.slf4j.slf4j-log4j12                                      | 15058  |          |
| org.apache.logging.log4j.log4j-api                           | 5479   | ×         |
| org.slf4j.log4j-over-slf4j                                   | 2877   | ×         |
| org.ops4j.pax.logging.pax-logging-api                        | 853    | ×         |
| org.apache.logging.log4j.log4j-to-slf4j                      | 273    | ×         |
| log4j.apache-log4j-extras                                    | 236    | ×         |
| org.apache.log4j.wso2.log4j                                  | 182    | ×         |
| org.jboss.logging.jboss-logging-log4j                        | 158    | ×         |
| org.ops4j.pax.logging.pax-logging-service                    | 158    | ×         |
| org.apache.log4j.com.springsource.org.apache.log4j           | 126    | ×         |
| org.jclouds.driver.jclouds-log4j                             | 119    | ×         |
| apache-log4j.log4j                                           | 103    | ×         |
| org.apache.jclouds.driver.jclouds-log4j                      | 92     | ×         |
| org.apache.tomcat.embed.tomcat-embed-logging-log4j           | 73     | ×         |
| org.apache.logging.log4j.log4j-api-scala                     | 71     | ×         |
| org.springframework.boot.spring-boot-starter-log4j           | 69     | ×         |
| io.cloudsoft.jclouds.driver.jclouds-log4j                    | 68     | ×         |
| jboss.jboss-common-logging-log4j                             | 57     | ×         |
| io.confluent.confluent-log4j                                 | 44     | ×         |
| org.jboss.logmanager.log4j-jboss-logmanager                  | 41     | ×         |
| com.amysta.jclouds.driver.jclouds-log4j                      | 34     | ×         |
| org.jclouds.jclouds-log4j                                    | 28     | ×         |
| com.amazonaws.aws-lambda-java-log4j                          | 28     | ×         |
| jboss.jboss-logging-log4j                                    | 26     | ×         |
| org.apache.ignite.ignite-log4j                               | 24     | ×         |
| org.codehaus.plexus.plexus-log4j-logging                     | 22     | ×         |
| com.pyx4j.maven-plugin-log4j                                 | 21     | ×         |
| org.pentaho.di.plugins.kettle-log4j-core                     | 19     | ×         |
| org.slf4j.com.springsource.slf4j.log4j                       | 18     | ×         |
| com.weicoder.extend.log4j-extend                             | 17     | ×         |
| net.logstash.log4j.jsonevent-layout                          | 17     | ×         |
| pentaho-kettle.kettle5-log4j-plugin                          | 16     | ×         |
| org.apache.kafka.kafka-log4j-appender                        | 16     | ×         |
| com.butor.butor-log4j                                        | 15     | ×         |
| org.bgee.log4jdbc-log4j2.log4jdbc-log4j2-jdbc4.1             | 15     | ×         |
| cd.connect.common.connect-java-logging                       | 15     | ×         |
| org.eclipse.equinox.org.apache.log4j                         | 13     | ×         |
| com.weicoder.fork.log4j-jdk11                                | 12     | ×         |
| de.mindpipe.android.android-logging-log4j                    | 12     | ×         |
| com.cisco.oss.foundation.logging-log4j                       | 12     | ×         |
| com.typesafe.scalalogging-log4j                              | 10     | ×         |
| org.apache.knox.gateway-i18n-logging-log4j                   | 9      | ×         |
| org.jboss.logmanager.log4j2-jboss-logmanager                 | 9      | ×         |
| org.bgee.log4jdbc-log4j2.log4jdbc-log4j2-jdbc4               | 9      | ×         |
| com.logentries.logentries-appender                           | 9      | ×         |
| com.yammer.metrics.metrics-log4j                             | 8      | ×         |
| uk.gov.justice.utils.test-utils-logging-log4j                | 8      | ×         |
| cd.connect.common.connect-java-logging-log4j2                | 8      | ×         |
| de.dentrassi.elasticsearch.log4j2-mock                       | 8      | ×         |
| org.ops4j.pax.logging.log4j                                  | 7      | ×         |
| org.apache.logging.log4j.log4j-catalog-api                   | 7      | ×         |
| at.bestsolution.efxclipse.eclipse.org.apache.log4j           | 7      | ×         |
| com.codahale.metrics.metrics-log4j                           | 6      | ×         |
| net.sourceforge.openutils.openutils-log4j                    | 6      | ×         |
| org.gridgain.ignite-log4j                                    | 6      | ×         |
| com.aliyun.openservices.log-loghub-log4j-appender            | 6      | ×         |
| cn.home1.log4j2-config-test                                  | 6      | ×         |
| cn.home1.log4j2-test-config                                  | 6      | ×         |
| org.mod4j.org.eclipse.xtext.log4j                            | 5      | ×         |
| io.dropwizard.metrics.metrics-log4j                          | 5      | ×         |
| org.apache.ant.ant-apache-log4j                              | 5      | ×         |
| org.fusesource.insight.insight-log4j                         | 5      | ×         |
| org.jboss.logmanager.jboss-logmanager-log4j                  | 5      | ×         |
| com.oxygenxml.oxygen-patched-log4j                           | 5      | ×         |
| com.guicedee.services.log4j-core                             | 5      | ×         |
| at.bestsolution.efxclipse.eclipse.org.slf4j.log4j            | 5      | ×         |
| org.apache.directory.studio.org.apache.logging.log4j         | 5      | ×         |
| io.zipkin.brave.brave-context-log4j12                        | 5      | ×         |
| org.slf4j.slf4j-log4j13                                      | 5      | ×         |
| uk.org.mygrid.taverna.raven.raven-log4j                      | 4      | ×         |
| io.fabric8.insight.insight-log4j                             | 4      | ×         |
| io.confluent.confluent-log4j-extensions                      | 4      | ×         |
| at.bestsolution.efxclipse.rt.org.eclipse.fx.core.slf4j       | 4      | ×         |
| at.bestsolution.efxclipse.rt.org.eclipse.fx.core.log4j       | 4      | ×         |
| org.grails.grails-plugin-log4j                               | 4      | ×         |
| dk.sundhed.ehealth.fut-log4j2                                | 4      | ×         |
| cn.home1.log4j2-config-rolling                               | 4      | ×         |
| org.apache.log4j                                             | 3      | ×         |
| simple.android.log4j.log4j-android                           | 3      | ×         |
| org.arakhne.afc.bootique.bootique-log4j                      | 3      | ×         |
| io.bitsensor.plugins.bitsensor-log4j                         | 3      | ×         |
| com.getsentry.raven.raven-log4j                              | 3      | ×         |
| org.apache.activemq.activemq-log4j-appender                  | 3      | ×         |
| com.google.flogger.flogger-log4j-backend                     | 3      | ×         |
| org.springframework.osgi.log4j.osgi                          | 3      | ×         |
| org.apache.log4j.org.apache.log4j                            | 3      | ×         |
| io.prometheus.simpleclient_log4j                             | 3      | ×         |
| de.huxhorn.lilith.de.huxhorn.lilith.log4j.throwable          | 3      | ×         |
| org.talend.daikon.audit-log4j2                               | 3      | ×         |
| org.apache.logging.log4j                                     | 2      | ×         |
| org.wso2.shade.log4j.log4j-shaded                            | 2      | ×         |
| uk.co.nichesolutions.logging.log4j.log4j-api                 | 2      | ×         |
| org.randomcoder.randomcoder-log4j-systemd-journal            | 2      | ×         |
| com.openhtmltopdf.openhtmltopdf-log4j                        | 2      | ×         |
| io.lighty.resources.log4j-properties                         | 2      | ×         |
| io.tracee.backend.tracee-log4j                               | 2      | ×         |
| net.kencochrane.raven.raven-log4j                            | 2      | ×         |
| wtf.metio.yosql.logging.yosql-logging-log4j                  | 2      | ×         |
| uk.org.simonsite.log4j-rolling-appender                      | 2      | ×         |
| plexus.plexus-log4j-logging                                  | 2      | ×         |
| org.ow2.monolog.monolog-wrapper-log4j                        | 2      | ×         |
| fr.jrds.jrds-log4j                                           | 2      | ×         |
| net.sf.taverna.t2.infrastructure.raven-log4j                 | 2      | ×         |
| de.taimos.daemon-framework-log4j                             | 2      | ×         |
| ant.ant-apache-log4j                                         | 2      | ×         |
| org.apache.isis.core.isis-core-log4j                         | 2      | ×         |
| de.codecrafters.listenersupport.failurestrategy-log4j        | 2      | ×         |
| com.ning.jetty.ning-service-skeleton-log4j                   | 2      | ×         |
| org.apache.samza.samza-log4j                                 | 2      | ×         |
| com.googlecode.kevinarpe-papaya.kevinarpe-papaya-testing-log4j | 2      | ×         |
| com.carrotgarden.log.carrot-log4j-aws-sns-pax                | 2      | ×         |
| org.mortbay.jetty.testwars.test-war-log4j_1.2.15             | 2      | ×         |
| se.fnord.log4j2-logstash-taggedmessage                       | 2      | ×         |
| se.fnord.log4j2-tagged-message                               | 2      | ×         |
| cn.home1.log4j2-rolling-config                               | 2      | ×         |
| org.hotswapagent.hotswap-agent-log4j2-plugin                 | 2      | ×         |
| net.minecrell.terminalconsoleappender                        | 2      | ×         |
| at.willhaben.willtest.log4j                                  | 1      | ×         |
| com.github.albfernandez.log4j                                | 1      | ×         |
| com.jkoolcloud.tnt4j.logger.log4j                            | 1      | ×         |
| org.darkphoenixs.log4j                                       | 1      | ×         |
| org.xbib.elasticsearch.log4j                                 | 1      | ×         |
| com.opsbears.webcomponents.application.slf4j.log4j           | 1      | ×         |
| org.onap.aaf.inno.log4j                                      | 1      | ×         |
| log4j.log4j-patched                                          | 1      | ×         |
| jboss.logging.log4j.jboss-logging-log4j                      | 1      | ×         |
| uk.co.nichesolutions.logging.log4j.log4j-core                | 1      | ×         |
| de.huxhorn.lilith.de.huxhorn.lilith.log4j.xml                | 1      | ×         |
| com.ryantenney.log4j.redis-appender                          | 1      | ×         |
| org.wso2.appserver.shade.log4j.log4j-shaded                  | 1      | ×         |
| com.sumologic.plugins.log4j.sumo-log4j-appender              | 1      | ×         |
| com.dinstone.loghub.loghub-log4j                             | 1      | ×         |
| org.tinylog.log4j-facade                                     | 1      | ×         |
| com.facebook.jcommon.logging-log4j                           | 1      | ×         |
| org.prevayler.extras.prevayler-log4j                         | 1      | ×         |
| de.holisticon.util.tracee.backend.tracee-log4j               | 1      | ×         |
| org.arakhne.afc.slf4j.slf4j-log4j                            | 1      | ×         |
| io.avaje.log4j-ecs                                           | 1      | ×         |
| io.sentry.sentry-log4j                                       | 1      | ×         |
| org.gridgain.gridgain-log4j                                  | 1      | ×         |
| ch.qos.logback.log4j-bridge                                  | 1      | ×         |
| org.apache.geronimo.gshell.gshell-diet-log4j                 | 1      | ×         |
| org.onap.aaf.authz.aaf-misc-log4j                            | 1      | ×         |
| com.nesscomputing.testing.ness-log4j-config                  | 1      | ×         |
| com.navercorp.pinpoint.pinpoint-log4j-plugin                 | 1      | ×         |
| org.apache.dubbo.dubbo-container-log4j                       | 1      | ×         |
| com.github.seratch.taskun.taskun-log4j-extension             | 1      | ×         |
| org.pentaho.di.plugins.kettle5-log4j-plugin                  | 1      | ×         |
| com.alibaba.dubbo-container-log4j                            | 1      | ×         |
| com.gilt.flume.log4j-flume-appender                          | 1      | ×         |
| com.randomnoun.common.log4j-one                              | 1      | ×         |
| org.zenframework.z8.dependencies.commons.log4j-1.2.17        | 1      | ×         |
| org.jmxtrans.jmxtrans-output-log4j                           | 1      | ×         |
| io.liftwizard.liftwizard-metrics-reporter-log4j              | 1      | ×         |
| com.tuuzed.common.logger-log4j                               | 1      | ×         |
| com.carrotgarden.log.carrot-log4j-aws-sns                    | 1      | ×         |
| org.netbeans.external.log4j-1.2.16                           | 1      | ×         |
| com.tencent.bk.base.datahub.kafka-log4j-appender             | 1      | ×         |
| io.opentelemetry.instrumentation.opentelemetry-log4j-2.13.2  | 1      | ×         |
| com.linkedin.kafka.kafka-log4j-appender                      | 1      | ×         |
| de.huxhorn.lilith.de.huxhorn.lilith.log4j.producer           | 1      | ×         |
| com.liferay.com.liferay.petra.log4j                          | 1      | ×         |
| de.huxhorn.lilith.de.huxhorn.lilith.log4j.converter          | 1      | ×         |
| org.apache.logging.log4j.adapters.log4j-to-slf4j             | 1      | ×         |
| com.anaptecs.jeaf.owalibs.org.apache.log4j                   | 1      | ×         |
| org.apache.logging.log4j.log4j-core-java9                    | 1      | ×         |
| io.boodskap.iot.ext.slf4j-boodskap-appender                  | 1      | ×         |
| com.truthbean.logger.log4j2-bridge                           | 1      | ×         |
| pl.wavesoftware.testing.log4j2                               | 1      | ×         |
| org.ops4j.pax.logging.pax-logging-log4j2-extra               | 1      | ×         |
| com.skyail.skyail-starter-log4j2                             | 1      | ×         |
| org.ops4j.pax.logging.pax-logging-sample-fragment-log4j2-h2  | 1      | ×         |
| io.axway.alf.alf-log4j2                                      | 1      | ×         |
| com.truthbean.log4j2-bridge                                  | 1      | ×         |
| com.googlecode.openbox.log                                   | 1      | ×         |
| com.vlkan.log4j2.log4j2-redis-appender                       | 1      | ×         |
| com.github.rocketraman.bootable.boot-logging-log4j2          | 1      | ×         |
| com.truthbean.logger.logger-to-log4j2                        | 1      | ×         |
| com.visionarts.lambda-log4j2                                 | 1      | ×         |
| com.mariocairone.log4j2-masking-policy-api                   | 1      | ×         |
| com.openjad.logger.openjad-logger-log4j2                     | 1      | ×         |
| pw.krejci.tracedepth-log4j2-plugin                           | 1      | ×         |
| de.huxhorn.lilith.de.huxhorn.lilith.log4j2.producer          | 1      | ×         |
| com.microsoft.azure.applicationinsights-logging-log4j2       | 1      | ×         |
| org.apache.logging.log4j.log4j2-stacktrace-origins           | 1      | ×         |
| com.github.vindell.spring-boot-starter-log4j2-plus           | 1      | ×         |
| com.github.vindell.spring-boot-starter-log4j2-biz            | 1      | ×         |
| cn.home1.oss-lib-log4j2-spring-boot-1.4.1.RELEASE            | 1      | ×         |
| net.savantly.log4j2.extended-jsonlayout-spring-auth          | 1      | ×         |
| com.lowagie.org.springframework.boot.spring-boot-starter-log4j2 | 1      | ×         |
| com.onloupe.loupe-log4j2-support                             | 1      | ×         |
| nz.net.osnz.composite.composite-logging-logback              | 1      | ×         |
| com.meituan.inf.xmd-log4j2                                   | 1      | ×         |
| com.therealvan.log4j-s3-search                               | 1      | ×         |
| nz.net.osnz.common.cloud-log4j2-over-slf4j-appender          | 1      | ×         |
| org.wso2.carbon.org.wso2.carbon.pax-logging-log4j2-plugins   | 1      | ×         |
| dk.sundhed.ehealth.logging.fut-log4j2-servlet-filter         | 1      | ×         |
| org.wso2.ei.org.wso2.micro.integrator.log4j2.plugins         | 1      | ×         |
| org.javastack.tomcat-juli-log4j2                             | 1      | ×         |
| io.symphonia.log4j2-json-helper                              | 1      | ×         |
| com.tersesystems.blacklite.blacklite-log4j2-codec-zstd       | 1      | ×         |
| se.fnord.log4j2-logstash-bom                                 | 1      | ×         |
| com.future94.alarm-log-examples-spring-mvc-log4j2            | 1      | ×         |
| nz.net.osnz.composite.composite-spring-boot-log4j2           | 1      | ×         |
| com.future94.alarm-log-examples-spring-boot-log4j2           | 1      | ×         |
| opentoutatice-ecm.log4j2.opentoutatice-log4j2-parent         | 1      | ×         |
| com.github.cafapi.logging.caf-logging-log4j2                 | 1      | ×         |
| com.synaptix.guice-log4j2                                    | 1      | ×         |
| cn.sunline.clhd.admin-sunlog-log4j2                          | 1      | ×         |
| io.paulbaker.shaded-log4j2-cachefile-transformer.io.paulbaker.shaded-log4j2-cachefile-transformer.gradle.plugin | 1      | ×         |
| com.taobao.middleware.logger.slf4j.log4j2.test               | 1      | ×         |
| com.rapid7.r7insight_java                                    | 1      | ×         |
| org.apache.meecrowave.meecrowave                             | 1      | ×         |
| com.idea-aedi.log4j2-defender                                | 1      | ×         |
| se.fnord.log4j2-logstash-reactor                             | 1      | ×         |
| nl.talsmasoftware.context.log4j2-propagation                 | 1      | ×         |
| com.vlkan.log4j2.log4j2-redis-appender-fatjar                | 1      | ×         |
| se.fnord.log4j2-logstash-layout                              | 1      | ×         |
| cn.home1.log-config.log4j2-test-config                       | 1      | ×         |
| pl.coffeepower.log4j.dynatrace-log4j2-appender               | 1      | ×         |
| net.dreamlu.mica-log4j2                                      | 1      | ×         |