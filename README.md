  ☆ノノハ
  从*’w’)
(つactorsと) [![Build Status](https://secure.travis-ci.org/plokhotnyuk/actors.png)](http://travis-ci.org/plokhotnyuk/actors)

Evaluation of API and performance of different actor libraries

## Hardware required

CPU: 2 cores or more
RAM: min 6Gb (for JDK 64-bit) or min 3Gb (for JDK 32-bit)

## Software installed required

JDK: 1.7.0_x or newer (can require of removing of some unsupported JVM options from test configuration)
Maven: 3.0.4 (or sbt: 0.12.1)

## Building & running benchmarks

Use following command-line instructions for JDK 64-bit:
mvn -B clean install >outX.txt (or sbt clean test >outX.txt)
For JDK 32-bit use the jdk32 profile:
mvn -B clean install -P jdk32 >outX.txt
For JRockit 64-bit use the jrockit64 profile:
mvn -B clean install -P jrockit64 >outX.txt

## Test result descriptions

out1.txt
Intel(R) Core(TM) i7-2640M CPU @ 2.80GHz (max 3.50GHz), RAM 12Gb DDR3-1333, Windows 7 sp1, JDK 1.7.0_10-b18 64-bit

out2.txt (with 2Gb of max heap size)
Intel(R) Core(TM)2 Duo CPU E6850 @ 3.00GHz, RAM 4Gb DDR2-800, Windows 7 sp1, JDK 1.7.0_10-b18 64-bit

out3.txt
Intel(R) Core(TM) i5-3570 CPU @ 3.40GHz (max 3.80GHz), RAM 16Gb DDR3-1333, Ubuntu 12.04, JDK 1.7.0_04-b20 64-bit