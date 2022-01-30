# Minecraft Servers Listing - Documentation

## Summary 
* Base URL and Headers
* **GET** Endpoints
  
-----

### Base URL and Headers

```diff
+ Base url : https://api.mcserverslisting.net
+ Headers: "Content-Type": "Application/json"
```

### **GET** Endpoints

-----

#### `GET /votes/:serverID/username`
* Get vote status of by providing server id and username
    * Username is player username provided on vote
        * example: `HiiZun`
    * Server id is the id provided by website
        * example: `15cf1cdb-a5c7-494c-8593-2cb8f311729f`

* Example of response
```json
    {
        voter: "HiiZun",
        server: "15cf1cdb-a5c7-494c-8593-2cb8f311729",
        hasVoted: true,
        latestVote: 1643455981456,
        votes: 6
    }
```
