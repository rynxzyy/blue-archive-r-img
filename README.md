# Blue Archive Random Images

This repository is simply for storing random images of Blue Archive characters. No fancy functions here!

## Why?

Because sometimes you just want to look at cute pictures from [Blue Archive](https://bluearchive.nexon.com/) without having to scour the entire internet.

## How to use?

1.  **View images:** The images are listed in the `links.json` file.
2.  **Access images with code:** You can fetch the images using the `links.json` file (see JavaScript example below).
3.  **Add images:** Add image links and their source information to `links.json` and make a pull request (see [Contributing])!

## Using `links.json` (JavaScript Example)

```javascript
const axios = require('axios');

axios.get('https://raw.githubusercontent.com/rynxzyy/blue-archive-r-img/refs/heads/main/links.json')
  .then(response => {
    const imageData = response.data;
    imageData.forEach(item => {
      console.log("URL:", item.url);
    });
  })
  .catch(error => {
    console.error("Error fetching image URLs:", error);
  });
```

## Contributing

Feel free to contribute! The more images, the merrier. Please make sure the images are:

*   From Blue Archive.
*   Safe for work (SFW).
*   Decent quality.

## License

All images belong to their respective creators and publishers (Nexon, Yostar, etc.). This repository is just for non-commercial fun.
