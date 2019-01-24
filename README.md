Stash
>persistent `dict`, backed-up by SQLite and pickle. Support py2.7 or py3.x

## Recommend:
Keys are arbitrary strings,values arbitrary pickle-able objects.

## Usage:
`pip install six` for Python compatibility

> I use this to save program running state or data in memory when the program stop accidentally

```
stash = Stash('sss.sqlite', table_name='ss')
stash["foo"] = "fuck"
stash['和谐'] = '健康'
del stash["foo"]
del stash["15"]
del stash['和谐']
```

More usage refer to **stash.py**

## Features
- Use `cPickle` with the highest protocol for Values
- Support for **multiple tables** in the same database file.

## Inspire

- [sqlite3dbm](https://github.com/Yelp/sqlite3dbm) I use it in py2.7 project which imitate `shelve` and mix `sqlite3`
- [sqlitedict](https://github.com/RaRe-Technologies/sqlitedict) `dict` mix `sqlite3` and `pickle`
- [sqlite_dbm](https://github.com/imbolc/sqlite_dbm)

