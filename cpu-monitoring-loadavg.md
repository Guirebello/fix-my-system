
# Meaning of the /proc/loadavg file
the file `/proc/loadavg` is constantly being updated by the system, and has 5 fields giving some system information.

- **1º, 2º, 3º fields**
	- five the respective 1 minute, 5 minutes and 15 minutes load average of the cpu. this information can be interpreted by the number of cores that are being used at the moment (virtual cores also count) so if we have a 20 total cores a loadavg of 1~2 means that not a lot of cpu is being used at the moment
- **4º field**
	- This field is typically displayed in the format `running/total` (e.g., `2/451`). Can be used to give you an idea of system activity
	- *Before the slash*: The number of processes currently running or actively scheduled.
	- *After the slash:* The total number of processes in the system at that moment.
- **5º field**
	- Last process ID (PID)

```
Example values of /proc/loadavg file:

0.22 0.34 0.35 5/916 21119
```

### Useful Links
- [Linux Load averages](https://www.brendangregg.com/blog/2017-08-08/linux-load-averages.html)
- [Calculating cpu usage based on /proc/loadavg and /proc/stat](https://stackoverflow.com/questions/9229333/how-to-get-overall-cpu-usage-e-g-57-on-linux)
