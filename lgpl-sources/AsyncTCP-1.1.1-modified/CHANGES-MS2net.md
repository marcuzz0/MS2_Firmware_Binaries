# Changes made for the MS2net firmware

This is AsyncTCP 1.1.1 by Hristo Gochkov (LGPL-3.0), modified for the MS2net firmware:

- `asyncTcpCloseAllClients()`: closes every open connection in an orderly way, so that the web
  server of the configuration page can be stopped without restarting the station;
- `asyncTcpStopTask()`: stops the library's task, so that its memory is given back when the
  configuration page is closed;
- the stack of that task raised to 8 KB;
- `SO_REUSEADDR` on the listening socket, so that the page can be opened again right away.
