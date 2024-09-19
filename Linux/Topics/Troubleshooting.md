# Boot Issue Troubleshooting

### Viewing the boot logs after a crash.

`cat /var/log/boot.log`
`tail /var/log/boot.log`

### Viewing Journal Logs

`jounralctl`

Running the command prints the SystemD logs.

*Might not be useful if there are no journal logs. Not certain what generates a journal log.*