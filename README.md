==========

Quick start: evaluate the proposed framework

1. Build ROS2 real-time application pendulum_demo

```
$ cd apps-to-trace/Pendulum_bestEffort_100
$ ./rebuild.sh
```

2. Launch pendulum_demo and start monitoring with the proposed framework

```
$ cd auto-tracer
$ ./launch-host-pendulum_demo.sh
```

==========

File list under auto-tracer/:

bcc-script.py: Main tracing frontend program  
ros2_tracing: ROS2 package for user-space tracing  
libfastrtps-with-thread-name: Patched FastDDS library with named internal threads  
post-process.py: Main postprocess script  
babeltrace2-plugins: Babeltrace2 plugin for postprocess  
bcc_log.chart.py: Sample plugin for Netdata  

==========

trace-data.zip: Trace files of performance issues discussed in the paper.
