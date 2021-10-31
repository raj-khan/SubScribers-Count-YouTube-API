# YouTube-API-Subscriber-Count
Sometimes we need YouTube channels Total Subscriber, Total videos, total views, this will help you to find those details.

![Logo](https://josephmuciraexclusives.com/wp-content/uploads/2019/08/YouTube-Data-API-Overview.jpg)



## Requirements

 - [Google Developers Account](https://developers.google.com/)
 - [Project using YouTube API V3](https://developers.google.com/youtube/v3)
 - [API Key & Auth Key](https://developers.google.com/youtube/v3/getting-started)


## API Reference

#### Get details

```http
  GET https://www.googleapis.com/youtube/v3/channels?part=statistics&id=$[channelID]]&key=${API KEY}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `API KEY` | `string` | **Required**. Your API key |
| `channelID` | `string` | **Required**. Your YouTube Channel ID|






## Demo

http://raajkhan.com/projects/api/youtube-sub


## FAQ

#### How to find API KEY?

You need to create a google developers account, then craete a project using YouTube API v3. In credential section you can generate API.

#### How to find YouTube channel ID?

While playing any youtube video if you click on this YouTube channel you can find the user ID in the browser url section.


## Tech Stack

JavaScript, HTML, Google Developers API

## Support

For support, email meherullah97@gmail.com.


## Code/Examples

```javascript
fetch(`https://www.googleapis.com/youtube/v3/channels?part=statistics&id=['CHANNEL ID']&key=[API KEY]`)
    .then(response => {
        return response.json()
    })
    .then(data => {
    console.log(data);
})
```


## License

[GLWTPL](https://github.com/me-shaon/GLWTPL/blob/master/LICENSE)

