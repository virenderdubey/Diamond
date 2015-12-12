IPVSCollector
=====

Shells out to get ipvs statistics, which may or may not require sudo access

#### Dependencies

 * /usr/sbin/ipvsadmin


#### Options - [Generic Options](Configuration)

<table><tr><th>Setting</th><th>Default</th><th>Description</th><th>Type</th></tr>
<tr><td>bin</td><td>/usr/sbin/ipvsadm</td><td>Path to ipvsadm binary</td><td>str</td></tr>
<tr><td>byte_unit</td><td>byte</td><td>Default numeric output(s)</td><td>str</td></tr>
<tr><td>enabled</td><td>False</td><td>Enable collecting these metrics</td><td>bool</td></tr>
<tr><td>measure_collector_time</td><td>False</td><td>Collect the collector run time in ms</td><td>bool</td></tr>
<tr><td>metrics_blacklist</td><td>None</td><td>Regex to match metrics to block. Mutually exclusive with metrics_whitelist</td><td>NoneType</td></tr>
<tr><td>metrics_whitelist</td><td>None</td><td>Regex to match metrics to transmit. Mutually exclusive with metrics_blacklist</td><td>NoneType</td></tr>
<tr><td>sudo_cmd</td><td>/usr/bin/sudo</td><td>Path to sudo</td><td>str</td></tr>
<tr><td>use_sudo</td><td>True</td><td>Use sudo?</td><td>bool</td></tr>
</table>

#### Example Output

```
servers.hostname.ipvs.TCP_172_16_1_56:443.10_68_15_66:443.conns 59
servers.hostname.ipvs.TCP_172_16_1_56:443.10_68_15_66:443.outbytes 216873
servers.hostname.ipvs.TCP_172_16_1_56:443.total.conns 59
servers.hostname.ipvs.TCP_172_16_1_56:80.total.conns 116
```

### This file was generated from the python source
### Please edit the source to make changes
