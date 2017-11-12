Sat Nov 11 16:15:31 PST 2017

  * Download sunriise-export-0.0.1-SNAPSHOT-exec.zip

  * Unzip to get files
    ** sunriise-export-0.0.1-SNAPSHOT-exec.jar
    ** loader.properties  

  * To export to MDB

  * Create a file loader.properties (if not exist) in current directory. Add

loader.main: com.hungle.sunriise.export.ExportToMdb

  * Usage: java com.hungle.sunriise.export.ExportToMdb in.mny [password] out.mdb

  * For example:

$ java -jar sunriise-export-0.0.1-SNAPSHOT-exec.jar /tmp/sunset-sample-pwd.mny 123@abc! /tmp/sunset-sample-pwd.mdb 
0 [main] INFO  com.hungle.sunriise.export.ExportToMdb.main(ExportToMdb.java:381) - srcFile=/tmp/sunset-sample-pwd.mny
6 [main] INFO  com.hungle.sunriise.io.MnyDb.openDb(MnyDb.java:412) - # Opening dbFile=/tmp/sunset-sample-pwd.mny, readOnly=true, encrypted=true
1722 [main] INFO  com.hungle.sunriise.io.MnyDb.close(MnyDb.java:220) - Closing dbFile=/tmp/sunset-sample-pwd.mny
1732 [main] INFO  com.hungle.sunriise.export.ExportToMdb.main(ExportToMdb.java:386) - destFile=/tmp/sunset-sample-pwd.mdb
1732 [main] INFO  com.hungle.sunriise.export.ExportToMdb.main(ExportToMdb.java:387) - < DONE

