#### CLOCK_REALTIME and CLOCK_MONOTONIC

时钟可以是系统范围内的（system-wide）或者只是进程范围内的，系统范围内实时时钟（墙上时钟）是CLOCK_REALTIME。
而CLOCK_MONOTONIC是一重单调时钟，不能设置，但是可以通过adjtime进行增加，也就说他是单调递增的，只能增加不能减少。
CLOCK_REALTIME 和 CLOCK_MONOTONIC 都是一种clockid_t。
更多的man一下clock_gettime()。