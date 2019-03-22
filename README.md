# osql
OrientDB interactive terminal

```
(defacto) josephbylund@kadmin-XPS-15-9570:~/osql$ osql --dbname=game_of_thrones
WARNING: importing upstream pyorient, this will cause a socketerror on some query exceptions.
In [1]: select 1;
[
    {
        "1": 1
    }
]

In [2]: select * from v limit 1;
[
    {
        "Image": "Thomas-McCarthy-200.jpg",
        "Title": "Thomas McCarthy",
        "birthplace": "New Jersey, USA",
        "dateofbirth": "30 January, 1966",
        "job": "Director",
        "name": "Thomas McCarthy",
        "url": "http://gameofthrones.wikia.com/wiki/Thomas McCarthy"
    }
]

In [3]: \timing
null
Time: 0.027 ms

In [4]: select max(name) from v;
[
    {
        "max": "Zoe Smedberg"
    }
]
Time: 49.419 ms
```
