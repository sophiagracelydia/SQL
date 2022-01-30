# Record Company Database
### 1. To change the column name into "Band Name"
[Solution](https://github.com/sophiagracelydia/SQL/blob/main/Record%20Company/solutions/1.Change%20Column%20Name.sql)
```sql
SELECT bands.name AS 'Band Name' FROM bands;
```
![image](https://user-images.githubusercontent.com/52828894/151688848-26d3cf96-e7db-43c9-a946-78045f91c2d7.png)


### 2. To select the oldest album
[Solution](https://github.com/sophiagracelydia/SQL/blob/main/Record%20Company/solutions/2.%20Select%20Oldest%20Album.sql)
```sql
SELECT * FROM albums
WHERE release_year IS NOT NULL
ORDER BY release_year
LIMIT 1;
```
![image](https://user-images.githubusercontent.com/52828894/151689196-4e92e188-10d0-42e5-adcd-3e18f3d82fe9.png)


### 3. Get all Bands that have Albums
[Solution](https://github.com/sophiagracelydia/SQL/blob/main/Record%20Company/solutions/3.%20Get%20all%20bands%20that%20have%20albums.sql)
```sql
SELECT DISTINCT bands.name AS 'Band Name'
FROM bands
JOIN albums ON bands.id = albums.band_id;
```
![image](https://user-images.githubusercontent.com/52828894/151694436-96358715-87fd-4bbc-bae1-3878a80867b2.png)
