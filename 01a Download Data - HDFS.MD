# Downloading airline delays data into HDFS

## Where are resources located?
Data can be downloaded at the following page: https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp?pn=1

Raw data should be available at this link: https://www.transtats.bts.gov/OT_Delay/ot_delaycause1.asp?display=download&pn=0&month=&year=

## Commands to download data into HDFS:
```
hadoop fs -mkdir /user/cloudera/airline_delays
hadoop fs -cd /user/cloudera/airline_delays
hadoop fs -wget https://www.transtats.bts.gov/OT_Delay/ot_delaycause1.asp?display=download&pn=0&month=&year=
```
