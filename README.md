# Pursuit-Core-Introduction-To-Networking-and-APIs-Lab

# Part One

Status Code Scavenger Hunt!

Use Postman to find each of the following HTTP codes:


1. 200
https://api.kanye.rest
200 OK message, GET request was successful.

1. 301




1. 400
 https://api.thecatapi.com/v1/images/searchs
 400 Bad Request Error - syntax error in URL
 (can be fixed by checking spelling and syntax in url)

1. 401
https://api.spotify.com/v1
401 Unauthorized error, "message": "No token provided"
(needs token to authorize access)

1. 403
 https://api.powerbi.com/v1.0/124edf19-b350-4797-aefc-3206115ffdb3/groups/
 403 Forbidden - i dont have access to this private group
 (unauthorized access)

1. 404
http://worldagnetwork.com/main
404 Not Found - /main does not exist 


1. 418
418 I'm a teapot - client error response code indicates that the server refuses to brew coffee because it is a teapot.

1. 500
https://httpstat.us/500
500 Internal Server Error - server 

For each of the questions below, write:

1. The website which generated the HTTP status code
2. A description of what the status code means
3. If an app you were writing encountered this status code, what would you do (if anything) to resolve any issues?


For reference, see:

https://en.wikipedia.org/wiki/List_of_HTTP_status_codes (Links to an external site.)
https://http.cat


# Part Two

API Scavenger Hunt!

For each of the questions below, identify a website and search query that will give you the appropriate JSON.  Paste the url and the json below.  Googling the category + API will generally take you to where you need.  Ex. https://lmgtfy.com/?q=cat+fact+api

1. A random cat fact
API:
https://catfact.ninja/fact

JSON:
{
"fact": "A commemorative tower was built in Scotland for a cat named Towser, who caught nearly 30,000 mice in her lifetime.",
"length": 114
}

1. A list of 150 random users in English.
API:
https://www.googleapis.com/admin/directory/v1/users

JSON:
{
"error": {
"errors": [
{
"domain": "global",
"reason": "required",
"message": "Login Required",
"locationType": "header",
"location": "Authorization"
}
],
"code": 401,
"message": "Login Required"
}
}


1. The current stock price of Microsoft. (IEX API)
API:
https://sandbox.iexapis.com/stable/stock/MSFT/quote?token=Tpk_bf7c800d40244b80b91c24dd593eb008



JSON:
{
"symbol": "MSFT",
"companyName": "Microsoft Corp.",
"primaryExchange": "NQDASA",
"calculationPrice": "tops",
"open": null,
"openTime": null,
"close": null,
"closeTime": null,
"high": null,
"low": null,
"latestPrice": 135.76,
"latestSource": "IEX real time price",
"latestTime": "2:35:20 PM",
"latestUpdate": 1620478911019,
"latestVolume": null,
"iexRealtimePrice": 139.12,
"iexRealtimeSize": 105,
"iexLastUpdated": 1598936366045,
"delayedPrice": null,
"delayedPriceTime": null,
"extendedPrice": null,
"extendedChange": null,
"extendedChangePercent": null,
"extendedPriceTime": null,
"previousClose": 138.15,
"previousVolume": null,
"change": 1.47,
"changePercent": 0.0114,
"volume": null,
"iexMarketPercent": 0.02930655072116735,
"iexVolume": 361161,
"avgTotalVolume": 27029866,
"iexBidPrice": 140.13,
"iexBidSize": 104,
"iexAskPrice": 142.55,
"iexAskSize": 100,
"marketCap": 1048437264765,
"peRatio": 27.7,
"week52High": 142.49,
"week52Low": 96.73,
"ytdChange": 0.331725547430799,
"lastTradeTime": 1582365160802,
"isUSMarketOpen": true
}


1. The 5 year history of Apple stock prices (IEX API)


1. All the Swift language repos on Github with Pursuit in their name
API:
https://api.github.com/search/repositories?q=pursuit-core+language:swift&sort=stars&order=desc

JSON:
"total_count": 45,
"incomplete_results": false,
"items": [
{
"id": 99703757,
"node_id": "MDEwOlJlcG9zaXRvcnk5OTcwMzc1Nw==",
"name": "Pursuit-Core-iOS",
"full_name": "joinpursuit/Pursuit-Core-iOS",
"private": false,
"owner": {
"login": "joinpursuit",
"id": 5825944,

...

1. A list of all Pokemon
API:
https://pokeapi.co/api/v2/pokemon/?limit=964

JSON:
"count": 964,
"next": null,
"previous": null,
"results": [
{
"name": "bulbasaur",
"url": "https://pokeapi.co/api/v2/pokemon/1/"
},
{
"name": "ivysaur",
"url": "https://pokeapi.co/api/v2/pokemon/2/"
},
{


1. A list of all items in Fortnite
API:
https://fortnite-api.theapinetwork.com/items/list

JSON:
{
"data": [
{
"itemId": "477f88c-eb310a8-234bcec-ccabb57",
"lastUpdate": 1557100802,
"item": {
"name": "Black Widow Outfit",
"description": "Whatever it takes.",
"cost": 1500,
"type": "outfit",
"rarity": "marvel",
"upcoming": false,
"costmeticId": "AthenaCharacter:cid_399_athena_commando_f_ashtonboardwalk",
"images": {
"icon": "https://fortnite-public-files.theapinetwork.com/outfit/c66dfd9c1fd49c4e28012294eaa1d779.png",
"featured": "https://fortnite-public-files.theapinetwork.com/featured/477f88c-eb310a8-234bcec-ccabb57.png",
"background": "https://fortnite-public-files.theapinetwork.com/image/477f88c-eb310a8-234bcec-ccabb57.png",
"information": "https://fortnite-public-files.theapinetwork.com/image/477f88c-eb310a8-234bcec-ccabb57/item.png"
},
"obtained": "1500",
"obtained_type": "vbucks",
"ratings": {
"avgStars": 4.26,
"totalPoints": 5922,
"numberVotes": 1391
}
}
},
{

1. A list of all Game of Thrones Episodes.
API:
api.got.show/api/show/episodes

JSON:
[
{
"written_by": [
"David Benioff",
"D.B. Weiss"
],
"characters": [
"Will",
"Waymar Royce",
"Gared",
"Wildling girl",
"White Walker 1",
"White Walker 2",
"Bran Stark",
"Jon Snow",
"Robb Stark",
"Catelyn Stark",
"Eddard Stark",
"Rickon Stark",
"Sansa Stark",
"Mordane",
"Arya Stark",
"Jeyne Poole",
"Rodrik Cassel",
"Jory Cassel",
"Theon Greyjoy",
"Lady",
"Grey Wind",
"Shaggydog",
"Summer",
"Nymeria",
"Ghost",
"Jaime Lannister",
"Cersei Lannister",
"Maester",
"Tommy",
"Joffrey Baratheon",
"Sandor Clegane",
"Preston Greenfield",
"Hodor",
"Mikken",
"Robert Baratheon",
"Tommen Baratheon",
"Myrcella Baratheon",
"Tyrion Lannister",
"Ros",
"Daenerys Targaryen",
"Viserys Targaryen",
"Pentoshi servant",
"Illyrio Mopatis",
"Khal",
"Qotho",
"Cohollo",
"Haggo",
"Benjen Stark",
"Jorah Mormont",
"Mago"
],
"deaths": [
"Waymar Royce",
"Gared",
"Will",
"Jon Arryn",
"Dothraki"
],
"places": [
"Beyond the Wall",
"In Pentos",
"In King's Landing",
"In the North",
"First",
"Deaths",
"Cast notes"
],
"_id": "5cc074bf04e71a0010b85a1a",
"title": "Winter Is Coming",
"season": 1,
"episode": 1,
"runtime": 62,
"directed_by": "Tim Van Patten",
"createdAt": "2019-04-24T14:37:51.759Z",
"updatedAt": "2019-04-24T14:37:51.759Z",
"__v": 0
},

1. A list of all songs with "Love" in the title.
API:
http://ws.audioscrobbler.com/2.0/?method=track.search&track=Love&api_key=7e102a7a374864e194aab0b8543ccb45&format=json

JSON:
{
"results": {
"opensearch:Query": {
"#text": "",
"role": "request",
"startPage": "1"
},
"opensearch:totalResults": "13246585",
"opensearch:startIndex": "0",
"opensearch:itemsPerPage": "30",
"trackmatches": {
"track": [
{
"name": "FAKE LOVE",
"artist": "BTS",
"url": "https://www.last.fm/music/BTS/_/FAKE+LOVE",
"streamable": "FIXME",
"listeners": "81770",
"image": [
{
"#text": "https://lastfm-img2.akamaized.net/i/u/34s/2a96cbd8b46e442fc41c2b86b821562f.png",
"size": "small"
},
{
"#text": "https://lastfm-img2.akamaized.net/i/u/64s/2a96cbd8b46e442fc41c2b86b821562f.png",
"size": "medium"
},
{
"#text": "https://lastfm-img2.akamaized.net/i/u/174s/2a96cbd8b46e442fc41c2b86b821562f.png",
"size": "large"
},
{
"#text": "https://lastfm-img2.akamaized.net/i/u/300x300/2a96cbd8b46e442fc41c2b86b821562f.png",
"size": "extralarge"
}
],
"mbid": ""
},

1. All information about Petyr Baelish from the Game of Thrones books
API:
https://www.anapioficeandfire.com/api/characters/823

JSON:
{
"url": "https://www.anapioficeandfire.com/api/characters/823",
"name": "Petyr Baelish",
"gender": "Male",
"culture": "Valemen",
"born": "In 268 AC, at the Fingers",
"died": "",
"titles": [
"Master of coin (formerly)",
"Lord Paramount of the Trident",
"Lord of Harrenhal",
"Lord Protector of the Vale"
],
"aliases": [
"Littlefinger"
],
"father": "",
"mother": "",
"spouse": "https://www.anapioficeandfire.com/api/characters/688",
"allegiances": [
"https://www.anapioficeandfire.com/api/houses/10",
"https://www.anapioficeandfire.com/api/houses/11"
],
"books": [
"https://www.anapioficeandfire.com/api/books/1",
"https://www.anapioficeandfire.com/api/books/2",
"https://www.anapioficeandfire.com/api/books/3",
"https://www.anapioficeandfire.com/api/books/5",
"https://www.anapioficeandfire.com/api/books/8"
],
"povBooks": [],
"tvSeries": [
"Season 1",
"Season 2",
"Season 3",
"Season 4",
"Season 5",
"Season 6"
],
"playedBy": [
"Aidan Gillen"
]
}

1. All the movies Leonardo Dicaprio has acted in
API: https://api.themoviedb.org/3/search/person?api_key=74faa787faa699b2a342dd3620deab63&language=en-US&query=Leonardo-Dicaprio&page=1&include_adult=false

JSON:
{
"page": 1,
"total_results": 1,
"total_pages": 1,
"results": [
{
"popularity": 14.293,
"known_for_department": "Acting",
"gender": 2,
"id": 6193,
"profile_path": "/aLUFp0zWpLVyIOgY0scIpuuKZLE.jpg",
"adult": false,
"known_for": [
{
"release_date": "2010-07-16",
"id": 27205,
"vote_count": 22884,
"video": false,
"media_type": "movie",
"vote_average": 8.3,
"title": "Inception",
"genre_ids": [
28,
12,
878
],
"original_title": "Inception",
"original_language": "en",
"adult": false,
"backdrop_path": "/s2bT29y0ngXxxu2IA8AOzzXTRhd.jpg",
"overview": "Cobb, a skilled thief who commits corporate espionage by infiltrating the subconscious of his targets is offered a chance to regain his old life as payment for a task considered to be impossible: \"inception\", the implantation of another person's idea into a target's subconscious.",
"poster_path": "/qmDpIHrmpJINaRKAfWQfftjCdyi.jpg"
},
{
"release_date": "2012-12-25",
"id": 68718,
"vote_count": 16183,
"video": false,
"media_type": "movie",
"vote_average": 8,
"title": "Django Unchained",
"genre_ids": [
18,
37
],
"original_title": "Django Unchained",
"original_language": "en",
"adult": false,
"backdrop_path": "/qUcmEqnzIwlwZxSyTf3WliSfAjJ.jpg",
"overview": "With the help of a German bounty hunter, a freed slave sets out to rescue his wife from a brutal Mississippi plantation owner.",
"poster_path": "/5WJnxuw41sddupf8cwOxYftuvJG.jpg"
},
{
"poster_path": "/kHXEpyfl6zqn8a6YuozZUujufXf.jpg",
"id": 597,
"vote_count": 14778,
"video": false,
"media_type": "movie",
"adult": false,
"backdrop_path": "/xqQztbT6KlPLQLlRtNHoXivEMZA.jpg",
"genre_ids": [
18,
10749,
53
],
"original_title": "Titanic",
"original_language": "en",
"title": "Titanic",
"vote_average": 7.8,
"overview": "101-year-old Rose DeWitt Bukater tells the story of her life aboard the Titanic, 84 years later. A young Rose boards the ship with her mother and fiancé. Meanwhile, Jack Dawson and Fabrizio De Rossi win third-class tickets aboard the ship. Rose tells the whole story from Titanic's departure through to its death—on its first and last voyage—on April 15, 1912.",
"release_date": "1997-12-19"
}
],
"name": "Leonardo DiCaprio"
}
]
}
