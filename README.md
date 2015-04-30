# sqlite

Cloned from https://android.googlesource.com/platform/external/sqlite.git.

The branch *research* is used to explore the sqlite things.

# sqlite error codes and messages

## Basic error codes

| Error constant | Error code | Error message |
| -------------- | ---------- | ------------- |
| SQLITE_OK | 0 | not an error |
| SQLITE_ERROR | 1 | SQL logic error or missing database |
| SQLITE_INTERNAL | 2 | unknown error |
| SQLITE_PERM | 3 | access permission denied |
| SQLITE_ABORT | 4 | callback requested query abort |
| SQLITE_BUSY | 5 | database is locked |
| SQLITE_LOCKED | 6 | database table is locked |
| SQLITE_NOMEM | 7 | out of memory |
| SQLITE_READONLY | 8 | attempt to write a readonly database |
| SQLITE_INTERRUPT | 9 | interrupted |
| SQLITE_IOERR | 10 | disk I/O error |
| SQLITE_CORRUPT | 11 | database disk image is malformed |
| SQLITE_NOTFOUND | 12 | unknown operation |
| SQLITE_FULL | 13 | database or disk is full |
| SQLITE_CANTOPEN | 14 | unable to open database file |
| SQLITE_PROTOCOL | 15 | locking protocol |
| SQLITE_EMPTY | 16 | table contains no data |
| SQLITE_SCHEMA | 17 | database schema has changed |
| SQLITE_TOOBIG | 18 | string or blob too big |
| SQLITE_CONSTRAINT | 19 | constraint failed |
| SQLITE_MISMATCH | 20 | datatype mismatch |
| SQLITE_MISUSE | 21 | library routine called out of sequence |
| SQLITE_NOLFS | 22 | large file support is disabled |
| SQLITE_AUTH | 23 | authorization denied |
| SQLITE_FORMAT | 24 | auxiliary database format error |
| SQLITE_RANGE | 25 | bind or column index out of range |
| SQLITE_NOTADB | 26 | file is encrypted or is not a database |
| SQLITE_NOTICE | 27 | unknown error |
| SQLITE_WARNING | 28 | unknown error |
| SQLITE_ROW | 100 | unknown error |
| SQLITE_DONE | 101 | unknown error |

## Extended error codes

| Error constant | Error code | Error message |
| -------------- | ---------- | ------------- |
| SQLITE_IOERR_READ | 266 | disk I/O error |
| SQLITE_IOERR_SHORT_READ | 522 | disk I/O error |
| SQLITE_IOERR_WRITE | 778 | disk I/O error |
| SQLITE_IOERR_FSYNC | 1034 | disk I/O error |
| SQLITE_IOERR_DIR_FSYNC | 1290 | disk I/O error |
| SQLITE_IOERR_TRUNCATE | 1546 | disk I/O error |
| SQLITE_IOERR_FSTAT | 1802 | disk I/O error |
| SQLITE_IOERR_UNLOCK | 2058 | disk I/O error |
| SQLITE_IOERR_RDLOCK | 2314 | disk I/O error |
| SQLITE_IOERR_DELETE | 2570 | disk I/O error |
| SQLITE_IOERR_BLOCKED | 2826 | disk I/O error |
| SQLITE_IOERR_NOMEM | 3082 | disk I/O error |
| SQLITE_IOERR_ACCESS | 3338 | disk I/O error |
| SQLITE_IOERR_CHECKRESERVEDLOCK | 3594 | disk I/O error |
| SQLITE_IOERR_LOCK | 3850 | disk I/O error |
| SQLITE_IOERR_CLOSE | 4106 | disk I/O error |
| SQLITE_IOERR_DIR_CLOSE | 4362 | disk I/O error |
| SQLITE_IOERR_SHMOPEN | 4618 | disk I/O error |
| SQLITE_IOERR_SHMSIZE | 4874 | disk I/O error |
| SQLITE_IOERR_SHMLOCK | 5130 | disk I/O error |
| SQLITE_IOERR_SHMMAP | 5386 | disk I/O error |
| SQLITE_IOERR_SEEK | 5642 | disk I/O error |
| SQLITE_IOERR_DELETE_NOENT | 5898 | disk I/O error |
| SQLITE_IOERR_MMAP | 6154 | disk I/O error |
| SQLITE_IOERR_GETTEMPPATH | 6410 | disk I/O error |
| SQLITE_IOERR_CONVPATH | 6666 | disk I/O error |
| SQLITE_LOCKED_SHAREDCACHE | 262 | database table is locked |
| SQLITE_BUSY_RECOVERY | 261 | database is locked |
| SQLITE_BUSY_SNAPSHOT | 517 | database is locked |
| SQLITE_CANTOPEN_NOTEMPDIR | 270 | unable to open database file |
| SQLITE_CANTOPEN_ISDIR | 526 | unable to open database file |
| SQLITE_CANTOPEN_FULLPATH | 782 | unable to open database file |
| SQLITE_CANTOPEN_CONVPATH | 1038 | unable to open database file |
| SQLITE_CORRUPT_VTAB | 267 | database disk image is malformed |
| SQLITE_READONLY_RECOVERY | 264 | attempt to write a readonly database |
| SQLITE_READONLY_CANTLOCK | 520 | attempt to write a readonly database |
| SQLITE_READONLY_ROLLBACK | 776 | attempt to write a readonly database |
| SQLITE_READONLY_DBMOVED | 1032 | attempt to write a readonly database |
| SQLITE_ABORT_ROLLBACK | 516 | abort due to ROLLBACK |
| SQLITE_CONSTRAINT_CHECK | 275 | constraint failed |
| SQLITE_CONSTRAINT_COMMITHOOK | 531 | constraint failed |
| SQLITE_CONSTRAINT_FOREIGNKEY | 787 | constraint failed |
| SQLITE_CONSTRAINT_FUNCTION | 1043 | constraint failed |
| SQLITE_CONSTRAINT_NOTNULL | 1299 | constraint failed |
| SQLITE_CONSTRAINT_PRIMARYKEY | 1555 | constraint failed |
| SQLITE_CONSTRAINT_TRIGGER | 1811 | constraint failed |
| SQLITE_CONSTRAINT_UNIQUE | 2067 | constraint failed |
| SQLITE_CONSTRAINT_VTAB | 2323 | constraint failed |
| SQLITE_CONSTRAINT_ROWID | 2579 | constraint failed |
| SQLITE_NOTICE_RECOVER_WAL | 283 | unknown error |
| SQLITE_NOTICE_RECOVER_ROLLBACK | 539 | unknown error |
| SQLITE_WARNING_AUTOINDEX | 284 | unknown error |
| SQLITE_AUTH_USER | 279 | authorization denied |
