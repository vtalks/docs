# Backup

How to backup the database manually. Works on development and
production.

To import the database from a backup execute:

```bash
compose exec postgres /restoredb.sh
```

To export the database execute:

```bash
compose exec postgres /dumpdb.sh
```