# Twitter-proxy

Allows you to make requests to the Twitter API by enabling proxy settings on the mobile app.

## Install
`Clone Repository`
`npm install`

## Getting started

0. Create an app on [dev twitter](https://developer.twitter.com/)

0. Create a json configuration file `config.json` in project root, containing your app api key,secret, and port:

    ```json
    {
      "apiKey": "<paste api key here>",
      "apiSecret": "<paste api secret here>",
      "port": "<custom port here>"
    }
    ```


0. Run the app using: 
    ```
    $ npm start ./config.json
    ```

You can now make requests to Twitter APIs by substituting Twitter base URL with `http://localhost:port`, where `port`
denotes the port that was assigned to this server. As an example, if a prior direct request to Twitter pointed to

```
https://api.twitter.com/1.1/search/tweets.json?q=%40twitterdev
```

now, having to pass through the proxy, it points to

```
http://localhost:port/1.1/search/tweets.json?q=%40twitterdev
```


## License

[MIT License](http://phuu.mit-license.org/)

