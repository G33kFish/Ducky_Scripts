What it does

Flushes DNS

Renews IP

Resets Winsock

Clears temp files

Restarts Spooler + Windows Update (wuauserv)

Runs SFC and DISM

Generates a connectivity report

Opens relevant support pages

Prompts the tech: Printer / Network / Windows Update (menu)

Saves a timestamped log + exit-code summary and attempts to copy it to the Bunny storage

This is for authorized IT/admin use on systems you’re permitted to service.


What you get (artifacts)

On the target (always):

%TEMP%\HelpdeskToolkit_<timestamp>\

HelpdeskToolkit_<HOST>_<timestamp>.log

HelpdeskToolkit_<HOST>_<timestamp>_summary.txt

Connectivity_<HOST>_<timestamp>.txt (if network/all)

Attempted copy to Bunny storage:

X:\loot\HelpdeskToolkit_<HOST>_<timestamp>\ (if a matching volume label is detected)

Notes / tuning

UAC: ALT y is best on US keyboard + default UAC dialog. If your environment uses different UAC behavior or non-US layout, tell me and I’ll adjust.

Timing: If machines are slow, increase the first DELAY 6000 to 8000–12000.

Support pages: I used Microsoft support links; you can swap to your internal KB URLs.

If you want, I can also provide a three-payload version (Printer/Network/WU as separate payload.txt switch positions) which is even more reliable than an interactive prompt.
