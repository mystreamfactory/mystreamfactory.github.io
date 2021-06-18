# Automatic website for streaming movies and TV series

![Automatic website for streaming movies and TV series](https://mystreamfactory.github.io/list.png)

## Movie/TV Streaming Website (API DOODSTREAM)

![Movie/TV Streaming Website via an API DOODSTREAM](https://mystreamfactory.github.io/doodstream.png)

- [https://ok.ru/video/2582006401642](https://ok.ru/video/2582006401642)
- [https://streamable.com/i1c2pf](https://streamable.com/i1c2pf)

#### Automating (API DOODSTREAM)

```
# --------------- DOODSTREAM (MOVIE) ---------------

1 ~ https://doodapi.com/api/folder/list?key=DOOD_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=af6887753365e14160254ac7f4345dd2 ~ movie_results.0.title <> title_en! <> 1 ~ movie_results.0.poster_path <> poster <> 1 ~ movie_results.0.id <> custom.tmdb_id <> 1 ~ "movie" <> type ~ movie_results.0.backdrop_path <> pictures <> 1 ~ movie_results.0.release_date <> premiere <> 1 ~ movie_results.0.overview <> description <> 1 ~ movie_results.0.vote_average <> rating <> 1 ~ movie_results.0.vote_count <> vote <> 1

# --------------- DOODSTREAM (TV) ---------------

1 ~ https://doodapi.com/api/folder/list?key=DOOD_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=af6887753365e14160254ac7f4345dd2 ~ tv_results.0.name <> title_en! <> 1 ~ tv_results.0.poster_path <> poster <> 1 ~ tv_results.0.id <> custom.tmdb_id <> 1 ~ "tv" <> type ~ tv_results.0.backdrop_path <> pictures <> 1 ~ tv_results.0.first_air_date <> premiere <> 1 ~ tv_results.0.origin_country.0 <> country <> 1 ~ tv_results.0.overview <> description <> 1 ~ tv_results.0.vote_average <> rating <> 1 ~ tv_results.0.vote_count <> vote <> 1

# --------------- DOODSTREAM (EMBED) ---------------

1 ~ https://doodapi.com/api/folder/list?key=DOOD_KEY ~ result.files ~ [url] <> result.folders <> fld_id <> "https://doodapi.com/api/file/list?key=DOOD_KEY&fld_id=_VALUE_" ~ file_code <> custom.player1 <> <> <> "DOODSTREAM https://dood.to/e/_VALUE_" ~ title <> custom.season ~ title <> custom.episode ~ additional_info.name <> custom.imdb_id

```

## Movie/TV Streaming Website (API NINJASTREAM)

![Movie/TV Streaming Website via an API NINJASTREAM](https://mystreamfactory.github.io/ninjastream.png)

- [https://ok.ru/video/2582021278314](https://ok.ru/video/2582021278314)
- [https://streamable.com/q1ukv7](https://streamable.com/q1ukv7)

#### Automating (API NINJASTREAM)

```
# --------------- NINJASTREAM (MOVIE) ---------------

1 ~ POST>https://api.ninjastream.to/api/folder/get?apiId=NINJA_ID&apiSecretId=NINJA_SECRET ~ result.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=9e43f45f94705cc8e1d5a0400d19a7b7 ~ movie_results.0.title <> title_en! <> 1 ~ movie_results.0.poster_path <> poster <> 1 ~ movie_results.0.id <> custom.tmdb_id <> 1 ~ "movie" <> type ~ movie_results.0.backdrop_path <> pictures <> 1 ~ movie_results.0.release_date <> premiere <> 1 ~ movie_results.0.overview <> description <> 1 ~ movie_results.0.vote_average <> rating <> 1 ~ movie_results.0.vote_count <> vote <> 1

# --------------- NINJASTREAM (TV) ---------------

1 ~ POST>https://api.ninjastream.to/api/folder/get?apiId=NINJA_ID&apiSecretId=NINJA_SECRET ~ result.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=9e43f45f94705cc8e1d5a0400d19a7b7 ~ tv_results.0.name <> title_en! <> 1 ~ tv_results.0.poster_path <> poster <> 1 ~ tv_results.0.id <> custom.tmdb_id <> 1 ~ "tv" <> type ~ tv_results.0.backdrop_path <> pictures <> 1 ~ tv_results.0.first_air_date <> premiere <> 1 ~ tv_results.0.origin_country.0 <> country <> 1 ~ tv_results.0.overview <> description <> 1 ~ tv_results.0.vote_average <> rating <> 1 ~ tv_results.0.vote_count <> vote <> 1

# --------------- NINJASTREAM (EMBED) ---------------

1 ~ POST>https://api.ninjastream.to/api/folder/get?apiId=NINJA_ID&apiSecretId=NINJA_SECRET ~ result.data ~ [url] <> result <> id <> "POST>https://api.ninjastream.to/api/file/get?apiId=NINJA_ID&apiSecretId=NINJA_SECRET&folder=_VALUE_" ~ hashid <> custom.player2 <> <> <> "NINJASTREAM https://ninjastream.to/watch/_VALUE_" ~ name <> custom.season ~ name <> custom.episode ~ additional_info.name <> custom.imdb_id

```

## Movie/TV Streaming Website (API STREAMSB)

![Movie/TV Streaming Website via an API STREAMSB](https://mystreamfactory.github.io/streamsb.png)

#### Automating (API STREAMSB)

- [https://ok.ru/video/2582024096362](https://ok.ru/video/2582024096362)
- [https://streamable.com/89b8qa](https://streamable.com/89b8qa)

```
# --------------- STREAMSB (MOVIE) ---------------

1 ~ https://streamsb.com/api/folder/list?key=STREAMSB_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=9e43f45f94705cc8e1d5a0400d19a7b7 ~ movie_results.0.title <> title_en! <> 1 ~ movie_results.0.poster_path <> poster <> 1 ~ movie_results.0.id <> custom.tmdb_id <> 1 ~ "movie" <> type ~ movie_results.0.backdrop_path <> pictures <> 1 ~ movie_results.0.release_date <> premiere <> 1 ~ movie_results.0.overview <> description <> 1 ~ movie_results.0.vote_average <> rating <> 1 ~ movie_results.0.vote_count <> vote <> 1

# --------------- STREAMSB (TV) ---------------

1 ~ https://streamsb.com/api/folder/list?key=STREAMSB_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=9e43f45f94705cc8e1d5a0400d19a7b7 ~ tv_results.0.name <> title_en! <> 1 ~ tv_results.0.poster_path <> poster <> 1 ~ tv_results.0.id <> custom.tmdb_id <> 1 ~ "tv" <> type ~ tv_results.0.backdrop_path <> pictures <> 1 ~ tv_results.0.first_air_date <> premiere <> 1 ~ tv_results.0.origin_country.0 <> country <> 1 ~ tv_results.0.overview <> description <> 1 ~ tv_results.0.vote_average <> rating <> 1 ~ tv_results.0.vote_count <> vote <> 1

# --------------- STREAMSB (EMBED) ---------------

1 ~ https://streamsb.com/api/folder/list?key=STREAMSB_KEY ~ result.files ~ [url] <> result.folders <> fld_id <> "https://streamsb.com/api/file/list?key=STREAMSB_KEY&per_page=200&fld_id=_VALUE_" ~ file_code <> custom.player3 <> <> <> "STREAMSB https://sbembed1.com/e/_VALUE_.html" ~ title <> custom.season ~ title <> custom.episode ~ additional_info.name <> custom.imdb_id

```

## Movie/TV Streaming Website (API STREAMTAPE)

![Movie/TV Streaming Website via an API STREAMTAPE](https://mystreamfactory.github.io/streamtape.png)

#### Automating (API STREAMTAPE)

- [https://ok.ru/video/2582024227434](https://ok.ru/video/2582024227434)
- [https://streamable.com/dmqame](https://streamable.com/dmqame)

```
# --------------- STREAMTAPE (MOVIE) ---------------

1 ~ https://api.streamtape.com/file/listfolder?login=STREAMTAPE_LOGIN&key=STREAMTAPE_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=9e43f45f94705cc8e1d5a0400d19a7b7 ~ movie_results.0.title <> title_en! <> 1 ~ movie_results.0.poster_path <> poster <> 1 ~ movie_results.0.id <> custom.tmdb_id <> 1 ~ "movie" <> type ~ movie_results.0.backdrop_path <> pictures <> 1 ~ movie_results.0.release_date <> premiere <> 1 ~ movie_results.0.overview <> description <> 1 ~ movie_results.0.vote_average <> rating <> 1 ~ movie_results.0.vote_count <> vote <> 1

# --------------- STREAMTAPE (TV) ---------------

1 ~ https://api.streamtape.com/file/listfolder?login=STREAMTAPE_LOGIN&key=STREAMTAPE_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=9e43f45f94705cc8e1d5a0400d19a7b7 ~ tv_results.0.name <> title_en! <> 1 ~ tv_results.0.poster_path <> poster <> 1 ~ tv_results.0.id <> custom.tmdb_id <> 1 ~ "tv" <> type ~ tv_results.0.backdrop_path <> pictures <> 1 ~ tv_results.0.first_air_date <> premiere <> 1 ~ tv_results.0.origin_country.0 <> country <> 1 ~ tv_results.0.overview <> description <> 1 ~ tv_results.0.vote_average <> rating <> 1 ~ tv_results.0.vote_count <> vote <> 1

# --------------- STREAMTAPE (EMBED) ---------------

1 ~ https://api.streamtape.com/file/listfolder?login=STREAMTAPE_LOGIN&key=STREAMTAPE_KEY ~ result.files ~ [url] <> result.folders <> id <> "https://api.streamtape.com/file/listfolder?login=STREAMTAPE_LOGIN&key=STREAMTAPE_KEY&folder=_VALUE_" ~ linkid <> custom.player4 <> <> <> "STREAMTAPE https://streamtape.com/e/_VALUE_" ~ name <> custom.season ~ name <> custom.episode ~ additional_info.name <> custom.imdb_id

```

## Movie/TV Streaming Website (API MIXDROP)

![Movie/TV Streaming Website via an API MIXDROP](https://mystreamfactory.github.io/mixdrop.png)

#### Automating (API MIXDROP)

- [https://ok.ru/video/2582018067050](https://ok.ru/video/2582018067050)
- [https://streamable.com/q5xoj4](https://streamable.com/q5xoj4)

```
# --------------- MIXDROP (MOVIE) ---------------

1 ~ https://api.mixdrop.co/folderlist?email=MIXDROP_EMAIL&key=MIXDROP_KEY ~ result.folders.0.title <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=269890f657dddf4635473cf4cf456576 ~ movie_results.0.title <> title_en! <> 1 ~ movie_results.0.poster_path <> poster <> 1 ~ movie_results.0.id <> custom.tmdb_id <> 1 ~ "movie" <> type ~ movie_results.0.backdrop_path <> pictures <> 1 ~ movie_results.0.release_date <> premiere <> 1 ~ movie_results.0.overview <> description <> 1 ~ movie_results.0.vote_average <> rating <> 1 ~ movie_results.0.vote_count <> vote <> 1

# --------------- MIXDROP (TV) ---------------

1 ~ https://api.mixdrop.co/folderlist?email=MIXDROP_EMAIL&key=MIXDROP_KEY ~ result.folders.0.title <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=269890f657dddf4635473cf4cf456576 ~ tv_results.0.name <> title_en! <> 1 ~ tv_results.0.poster_path <> poster <> 1 ~ tv_results.0.id <> custom.tmdb_id <> 1 ~ "tv" <> type ~ tv_results.0.backdrop_path <> pictures <> 1 ~ tv_results.0.first_air_date <> premiere <> 1 ~ tv_results.0.origin_country.0 <> country <> 1 ~ tv_results.0.overview <> description <> 1 ~ tv_results.0.vote_average <> rating <> 1 ~ tv_results.0.vote_count <> vote <> 1

# --------------- MIXDROP (EMBED) ---------------

1 ~ https://api.mixdrop.co/folderlist?email=MIXDROP_EMAIL&key=MIXDROP_KEY ~ result.files ~ [url] <> result.folders <> id <> "https://api.mixdrop.co/folderlist?email=MIXDROP_EMAIL&key=MIXDROP_KEY&id=_VALUE_" ~ fileref <> custom.player5 <> <> <> "MIXDROP https://mixdrop.sx/e/_VALUE_" ~ title <> custom.season ~ title <> custom.episode ~ additional_info.title <> custom.imdb_id

```

## Movie/TV Streaming Website (API UPSTREAM)

![Movie/TV Streaming Website via an API UPSTREAM](https://mystreamfactory.github.io/upstream.png)

#### Automating (API UPSTREAM)

- [https://ok.ru/video/2582024620650](https://ok.ru/video/2582024620650)
- [https://streamable.com/5r4lwl](https://streamable.com/5r4lwl)

```
# --------------- UPSTREAM (MOVIE) ---------------

1 ~ https://upstream.to/api/folder/list?key=UPSTREAM_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=269890f657dddf4635473cf4cf456576 ~ movie_results.0.title <> title_en! <> 1 ~ movie_results.0.poster_path <> poster <> 1 ~ movie_results.0.id <> custom.tmdb_id <> 1 ~ "movie" <> type ~ movie_results.0.backdrop_path <> pictures <> 1 ~ movie_results.0.release_date <> premiere <> 1 ~ movie_results.0.overview <> description <> 1 ~ movie_results.0.vote_average <> rating <> 1 ~ movie_results.0.vote_count <> vote <> 1

# --------------- UPSTREAM (TV) ---------------

1 ~ https://upstream.to/api/folder/list?key=UPSTREAM_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=269890f657dddf4635473cf4cf456576 ~ tv_results.0.name <> title_en! <> 1 ~ tv_results.0.poster_path <> poster <> 1 ~ tv_results.0.id <> custom.tmdb_id <> 1 ~ "tv" <> type ~ tv_results.0.backdrop_path <> pictures <> 1 ~ tv_results.0.first_air_date <> premiere <> 1 ~ tv_results.0.origin_country.0 <> country <> 1 ~ tv_results.0.overview <> description <> 1 ~ tv_results.0.vote_average <> rating <> 1 ~ tv_results.0.vote_count <> vote <> 1

# --------------- UPSTREAM (EMBED) ---------------

1 ~ https://upstream.to/api/folder/list?key=UPSTREAM_KEY ~ result.files ~ [url] <> result.folders <> fld_id <> "https://upstream.to/api/folder/list?key=UPSTREAM_KEY&fld_id=_VALUE_" ~ file_code <> custom.player6 <> <> <> "UPSTREAM https://upstream.to/embed-_VALUE_.html" ~ title <> custom.season ~ title <> custom.episode ~ additional_info.name <> custom.imdb_id

```

## Movie/TV Streaming Website (API VOE)

![Movie/TV Streaming Website via an API VOE](https://mystreamfactory.github.io/voe.png)

#### Automating (API VOE)

- [https://ok.ru/video/2582025144938](https://ok.ru/video/2582025144938)
- [https://streamable.com/bw8yia](https://streamable.com/bw8yia)

```
# --------------- VOE (MOVIE) ---------------

1 ~ https://voe.sx/api/folder/list?key=VOE_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=269890f657dddf4635473cf4cf456576 ~ movie_results.0.title <> title_en! <> 1 ~ movie_results.0.poster_path <> poster <> 1 ~ movie_results.0.id <> custom.tmdb_id <> 1 ~ "movie" <> type ~ movie_results.0.backdrop_path <> pictures <> 1 ~ movie_results.0.release_date <> premiere <> 1 ~ movie_results.0.overview <> description <> 1 ~ movie_results.0.vote_average <> rating <> 1 ~ movie_results.0.vote_count <> vote <> 1

# --------------- VOE (TV) ---------------

1 ~ https://voe.sx/api/folder/list?key=VOE_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=269890f657dddf4635473cf4cf456576 ~ tv_results.0.name <> title_en! <> 1 ~ tv_results.0.poster_path <> poster <> 1 ~ tv_results.0.id <> custom.tmdb_id <> 1 ~ "tv" <> type ~ tv_results.0.backdrop_path <> pictures <> 1 ~ tv_results.0.first_air_date <> premiere <> 1 ~ tv_results.0.origin_country.0 <> country <> 1 ~ tv_results.0.overview <> description <> 1 ~ tv_results.0.vote_average <> rating <> 1 ~ tv_results.0.vote_count <> vote <> 1

# --------------- VOE (EMBED) ---------------

1 ~ https://voe.sx/api/folder/list?key=VOE_KEY ~ result.files ~ [url] <> result.folders <> fld_id <> "https://voe.sx/api/folder/list?key=VOE_KEY&fld_id=_VALUE_" ~ file_code <> custom.player7 <> <> <> "VOE https://voe.sx/e/_VALUE_" ~ title <> custom.season ~ title <> custom.episode ~ additional_info.name <> custom.imdb_id

```

## Movie/TV Streaming Website (API PLAYTUBE)

![Movie/TV Streaming Website via an API PLAYTUBE](https://mystreamfactory.github.io/playtube.png)

#### Automating (API PLAYTUBE)

- [https://ok.ru/video/2582023506538](https://ok.ru/video/2582023506538)
- [https://streamable.com/qtwvru](https://streamable.com/qtwvru)

```
# --------------- PLAYTUBE (MOVIE) ---------------

1 ~ https://playtube.ws/api/folder/list?key=PLAYTUBE_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=269890f657dddf4635473cf4cf456576 ~ movie_results.0.title <> title_en! <> 1 ~ movie_results.0.poster_path <> poster <> 1 ~ movie_results.0.id <> custom.tmdb_id <> 1 ~ "movie" <> type ~ movie_results.0.backdrop_path <> pictures <> 1 ~ movie_results.0.release_date <> premiere <> 1 ~ movie_results.0.overview <> description <> 1 ~ movie_results.0.vote_average <> rating <> 1 ~ movie_results.0.vote_count <> vote <> 1

# --------------- PLAYTUBE (TV) ---------------

1 ~ https://playtube.ws/api/folder/list?key=PLAYTUBE_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=269890f657dddf4635473cf4cf456576 ~ tv_results.0.name <> title_en! <> 1 ~ tv_results.0.poster_path <> poster <> 1 ~ tv_results.0.id <> custom.tmdb_id <> 1 ~ "tv" <> type ~ tv_results.0.backdrop_path <> pictures <> 1 ~ tv_results.0.first_air_date <> premiere <> 1 ~ tv_results.0.origin_country.0 <> country <> 1 ~ tv_results.0.overview <> description <> 1 ~ tv_results.0.vote_average <> rating <> 1 ~ tv_results.0.vote_count <> vote <> 1

# --------------- PLAYTUBE (EMBED) ---------------

1 ~ https://playtube.ws/api/folder/list?key=PLAYTUBE_KEY ~ result.files ~ [url] <> result.folders <> fld_id <> "https://playtube.ws/api/folder/list?key=PLAYTUBE_KEY&fld_id=_VALUE_" ~ file_code <> custom.player8 <> <> <> "PLAYTUBE https://playtube.ws/embed-_VALUE_.html" ~ title <> custom.season ~ title <> custom.episode ~ additional_info.name <> custom.imdb_id

```

## Movie/TV Streaming Website (API STREAMON)

![Movie/TV Streaming Website via an API STREAMON](https://mystreamfactory.github.io/streamon.png)

#### Automating (API STREAMON)

- [https://ok.ru/video/2582023703146](https://ok.ru/video/2582023703146)
- [https://streamable.com/oaxjpf](https://streamable.com/oaxjpf)

```
# --------------- STREAMON (MOVIE) ---------------

1 ~ https://streamon.to/api/folder/list?key=STREAMON_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=af6887753365e14160254ac7f4345dd2 ~ movie_results.0.title <> title_en! <> 1 ~ movie_results.0.poster_path <> poster <> 1 ~ movie_results.0.id <> custom.tmdb_id <> 1 ~ "movie" <> type ~ movie_results.0.backdrop_path <> pictures <> 1 ~ movie_results.0.release_date <> premiere <> 1 ~ movie_results.0.overview <> description <> 1 ~ movie_results.0.vote_average <> rating <> 1 ~ movie_results.0.vote_count <> vote <> 1

# --------------- STREAMON (TV) ---------------

1 ~ https://streamon.to/api/folder/list?key=STREAMON_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=af6887753365e14160254ac7f4345dd2 ~ tv_results.0.name <> title_en! <> 1 ~ tv_results.0.poster_path <> poster <> 1 ~ tv_results.0.id <> custom.tmdb_id <> 1 ~ "tv" <> type ~ tv_results.0.backdrop_path <> pictures <> 1 ~ tv_results.0.first_air_date <> premiere <> 1 ~ tv_results.0.origin_country.0 <> country <> 1 ~ tv_results.0.overview <> description <> 1 ~ tv_results.0.vote_average <> rating <> 1 ~ tv_results.0.vote_count <> vote <> 1

# --------------- STREAMON (EMBED) ---------------

1 ~ https://streamon.to/api/folder/list?key=STREAMON_KEY ~ result.files ~ [url] <> result.folders <> fld_id <> "https://streamon.to/api/file/list?key=STREAMON_KEY&fld_id=_VALUE_" ~ file_code <> custom.player9 <> <> <> "STREAMON https://streamon.to/e/_VALUE_" ~ title <> custom.season ~ title <> custom.episode ~ additional_info.name <> custom.imdb_id

```

## Movie/TV Streaming Website (API UPVIDEO)

![Movie/TV Streaming Website via an API UPVIDEO](https://mystreamfactory.github.io/upvideo.png)

#### Automating (API UPVIDEO)

- [https://ok.ru/video/2582024948330](https://ok.ru/video/2582024948330)
- [https://streamable.com/7pm98n](https://streamable.com/7pm98n)

All players are already filled `custom.player{1-9}`

The current UPVIDEO player will be a spare option, if some of the main players fail, you can immediately replace on UPVIDEO.

You need to replace `custom.player1` on the number of the player, which has failed `custom.player{1-9}`

```
# --------------- UPVIDEO (MOVIE) ---------------

# 1 ~ https://upvideo.to/api/folder/list?key=UPVIDEO_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=af6887753365e14160254ac7f4345dd2 ~ movie_results.0.title <> title_en! <> 1 ~ movie_results.0.poster_path <> poster <> 1 ~ movie_results.0.id <> custom.tmdb_id <> 1 ~ "movie" <> type ~ movie_results.0.backdrop_path <> pictures <> 1 ~ movie_results.0.release_date <> premiere <> 1 ~ movie_results.0.overview <> description <> 1 ~ movie_results.0.vote_average <> rating <> 1 ~ movie_results.0.vote_count <> vote <> 1

# --------------- UPVIDEO (TV) ---------------

# 1 ~ https://upvideo.to/api/folder/list?key=UPVIDEO_KEY ~ result.folders.0.name <> custom.imdb_id ~ https://api.themoviedb.org/3/find/[imdb_id]?language=en&external_source=imdb_id&api_key=af6887753365e14160254ac7f4345dd2 ~ tv_results.0.name <> title_en! <> 1 ~ tv_results.0.poster_path <> poster <> 1 ~ tv_results.0.id <> custom.tmdb_id <> 1 ~ "tv" <> type ~ tv_results.0.backdrop_path <> pictures <> 1 ~ tv_results.0.first_air_date <> premiere <> 1 ~ tv_results.0.origin_country.0 <> country <> 1 ~ tv_results.0.overview <> description <> 1 ~ tv_results.0.vote_average <> rating <> 1 ~ tv_results.0.vote_count <> vote <> 1

# --------------- UPVIDEO (EMBED) ---------------

# 1 ~ https://upvideo.to/api/folder/list?key=UPVIDEO_KEY ~ result.files ~ [url] <> result.folders <> fld_id <> "https://upvideo.to/api/file/list?key=UPVIDEO_KEY&fld_id=_VALUE_" ~ file_code <> custom.player1 <> <> <> "UPVIDEO https://upvideo.to/e/_VALUE_" ~ title <> custom.season ~ title <> custom.episode ~ additional_info.name <> custom.imdb_id

```

## Full filling information about the Movies/TV

![Full filling information about the Movies/TV](https://mystreamfactory.github.io/info.png)

```
# --------------- UPDATING (INFO) ---------------

1 ~ lastmod_tv ~ custom.tmdb_id ~ https://api.themoviedb.org/3/tv/[id]?language=en-US&append_to_response=credits,external_ids&api_key=af6887753365e14160254ac7f4345dd2 ~ external_ids.imdb_id <> custom.imdb_id ~ "tv" <> type ~ backdrop_path <> pictures ~ poster_path <> poster ~ first_air_date <> premiere ~ name <> title_en ~ overview <> description ~ genres.0.name <> genre ~ credits.cast.0.name <> actor <> 5 ~ credits.crew.0.name <> director <> 5 <> job == Director ~ origin_country.0 <> country

1 ~ lastmod_movie ~ custom.tmdb_id ~ https://api.themoviedb.org/3/movie/[id]?language=en-US&append_to_response=credits,external_ids&api_key=af6887753365e14160254ac7f4345dd2 ~ external_ids.imdb_id <> custom.imdb_id ~ "movie" <> type ~ backdrop_path <> pictures ~ poster_path <> poster ~ release_date <> premiere ~ title <> title_en ~ overview <> description ~ genres.0.name <> genre ~ credits.cast.0.name <> actor <> 5 ~ credits.crew.0.name <> director <> 5 <> job == Director ~ production_countries.0.iso_3166_1 <> country

```

## Updating IMDB rating

```
# --------------- UPDATING (RATING) ---------------

0 ~ https://datasets.imdbws.com/title.ratings.tsv.gz ~ ~ ~ tconst <> custom.imdb_id ~ averageRating <> imdb_rating ~ numVotes <> imdb_vote

```
