# spark-twitter-named-entity

This is a fast **named entity extraction** module which listens to twitter stream and utilizes Spark Streaming.
For simplicity this project is listening to all user public stream and filtering based only on fortune 500 companies to get tweets related to corporates.

> Note: this does not perform recognition of named entities into classes like person, location or organization.


# Get Running
- Checkout the project
- Fill up your twitter keys in TwitterMain.scala
- Do maven build
- Download already trained model from [**here**](http://downloads.gate.ac.uk/twitie/gate-EN-twitter.model)
- Run TwitterMain.scala or do a spark-submit

# Sample Output Stream: 
(one row corresponds to each tweet)

```
Set(Microsoft Xbox)
Set(Jacob Johanssen, Facebook)
Set(Spotify, Google, iTunes, Apple Music)
Set(Russell Crowe, United Kingdom)
Set(JS, Facebook, NPM)
Set(National Anthem)
Set(EXO)
Set()
Set(Verizon Wireless Android Smartphone, Samsung N920 Galaxy)
Set(ProChat24 File)
Set(US Supreme Court)
Set(Dusshera)
Set(William Hill, Poker-Stars)
Set(Social Media Surveillance, Instagram Share Data)
Set(Jacob Osei Yeboah)
 .............continuous stream .....
```
