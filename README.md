# JMeter Performance Test: Banking Flow

Load test of a login → view account → transaction flow
against dummyjson.com (public demo API).

## Features
- Token correlation with JSON Extractor
- CSV parameterization (data/users.csv)
- Assertions (response code, JSON)
- Think time with Uniform Random Timer
- Transaction Controllers for business-level timings

## Run
jmeter -n -t test.jmx -l results.jtl -e -o report

## Sample results
5 users, 10s ramp-up: p95 = [x] ms, error rate = [x]%
(see sample-report/)

## Tools
JMeter 5.x, Java 8
