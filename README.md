# init system rosetta

## basic
| systemd  | runit                               |  openrc  | s6rc   |  sysvinit |
| :---     | :----                               |  :---    | :----  |  :---     |
| -----    | sv status /var/service/*            |  openrc  | s6rc   |  sysvinit |
| -----    | ln -s /etc/sv/ssh /var/service/ssh  |  openrc  | s6rc   |  sysvinit |
| -----    | rm /var/service/ssh                 |  openrc  | s6rc   |  sysvinit |
| -----    | sv down ssh                         |  openrc  | s6rc   |  sysvinit |
| -----    | sv up ssh                           |  openrc  | s6rc   |  sysvinit |
| -----    | sv restart ssh                      |  openrc  | s6rc   |  sysvinit |
| -----    | sv status ssh                       |  openrc  | s6rc   |  sysvinit |

## app
| systemd  | runit                               |  openrc  | s6rc   |  sysvinit |
| :---     | :----                               |  :---    | :----  |  :---     |
| [localectl]()    |                             |  openrc  | s6rc   |  sysvinit |
