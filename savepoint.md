* 出发一个savepoint[直接触发或者在cancel的时候触发]
停止程序： bin/flink cancel -s [targetDirectory] jobId [-yid yarnAppId] 

* 从指定的savepoint启动job
bin/flink run -s savepointPath [runArgs]


* 给每一个operator 起一个uid
