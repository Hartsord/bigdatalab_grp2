# Downloading airline delays data into HDFS

## Where are resources located?
Data can be downloaded at the following page: https://www.transtats.bts.gov/OT_Delay/OT_DelayCause1.asp?pn=1

Raw data should be available at this link: https://transtats.bts.gov/ftproot/TranStatsData/805001964_92018_4132_airline_delay_causes.zip

## Download data into Cloudera
```
mkdir ~/Downloads/airline_delays
cd ~/Downloads/airline_delays
wget https://transtats.bts.gov/ftproot/TranStatsData/805001964_92018_4132_airline_delay_causes.zip
```
Name of zip is "805001964_92018_4132_airline_delay_causes.zip"

## Load file into HDFS
```
hadoop fs -mkdir /user/cloudera/airline_delays
hadoop fs -put ~/Downloads/airline_delays/805001964_92018_4132_airline_delay_causes.zip /user/cloudera/airline_delays
