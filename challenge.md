# Coding Challenge - Software Engineer at Benu

Thank you for your time and interest in participating in this process. At Benu, we really care about new members joining the team and we want to make sure they fill right at home should they decide to join forces. This coding challenge is the chance we have to show you how a normal day might look like in our team. The objective here is to give you a feeling of what you will encounter so that you can decide for yourself whether that is something interesting for you. It is also an opportunity for us to understand more about your hard skills. With that said, we will not judge your experience purely on the results of this challenge as we understand there are a multitude of other things a Software Engineer is capable of that is outside of the scope of this challenge. We want you to have fun while doing this!

## Goal
We want to create an in-memory API Cache for [The Open Movie Database](https://www.omdbapi.com/) so that when 
we research a title once, it gets pushed to the cache and the following requests to the same title don't need to hit
the OMDB Api directly anymore.

Here is a sample API call with our API Key (feel free to use this api key):

```
curl -X GET "https://www.omdbapi.com/?apikey=15c2c91d&t=Iron+Man+3"

{
    Title: "Iron Man 3",
    Year: "2013",
    Rated: "PG-13",
    Released: "03 May 2013",
    Runtime: "130 min",
    Genre: "Action, Adventure, Sci-Fi",
    Director: "Shane Black",
    Writer: "Drew Pearce, Shane Black, Stan Lee",
    Actors: "Robert Downey Jr., Guy Pearce, Gwyneth Paltrow",
    Plot: "When Tony Stark's world is torn apart by a formidable terrorist called the Mandarin, he starts an odyssey of rebuilding and retribution.",
    Language: "English",
    Country: "United States",
    Awards: "Nominated for 1 Oscar. 20 wins & 63 nominations total",
    Poster: "https://m.media-amazon.com/images/M/MV5BMjE5MzcyNjk1M15BMl5BanBnXkFtZTcwMjQ4MjcxOQ@@._V1_SX300.jpg",
    Ratings: [
                {
                    Source: "Internet Movie Database",
                    Value: "7.1/10"
                },
                {
                    Source: "Rotten Tomatoes",
                    Value: "79%"
                },
                {
                    Source: "Metacritic",
                    Value: "62/100"
                }
            ],
    Metascore: "62",
    imdbRating: "7.1",
    imdbVotes: "892,130",
    imdbID: "tt1300854",
    Type: "movie",
    DVD: "08 Apr 2015",
    BoxOffice: "$409,013,994",
    Production: "N/A",
    Website: "N/A",
    Response: "True"
}
```

## Resources
We would love if you build this app using Spring Boot 3 and their caching library with EHcache. Here are some good starting points: 
- You can use the [Spring Initializr](https://start.spring.io/) to generate the barebones for you (with all the dependencies).  
- Here is a decent article on the basics of what we need: [Spring Boot Ehcache Example](https://www.baeldung.com/spring-boot-ehcache)
- You can use the Webclient to make the http requests to OMDB: [Spring 5 WebClient](https://www.baeldung.com/spring-5-webclient)


## Acceptance Criteria:
 - The app exposes a REST endpoint taking a movie title as a query parameter
 - Responses where the movie was not found should not be cached
 - The app exposes a REST endpoint to clear the cache

## Deliverables
It'd be amazing to have the following:
- Git repository where we can clone the code
- Dockerfile to run the service
- readme file explaining how to start the docker container and a sample CURL request to fetch movies by title

### Have fun, and thanks again for taking the time to do this!
Feel free to reach out if you have any questions! 
