commands and tools for JVM diagnostics are 

JVM Parameters : 
```bash
-Xmx512m


```

GUI Tools for JVM, heap and thread analysis 
- jconsole - light weight ( comes with jdk ) 
- visualvm - more indepth ( download separately )

```bash
# List all java processes
jcmd

# jcmd <PID> help
jcmd 12924 help

# Thread Dump
jcmd 12924 Thread.dump_to_file 12924_thread_dump.txt

jcmd 12924 Thread.print > 12924_thread_dump.txt

# Heap Info
jcmd 12924 GC.heap_info

jcmd 12924 GC.heap_dump /c/_GitRepos/TEMP/app_heap_dump.hprof

```

References : https://www.baeldung.com/running-jvm-diagnose