# Blue Archive Random Images

This repository is simply for storing random images of Blue Archive characters. No fancy functions here!

## Why?

Because sometimes you just want to look at cute pictures from [Blue Archive](https://bluearchive.nexon.com/) without having to scour the entire internet.

## How to use?

1.  **View images:** Browse the [`images`](./images) folder to see all the images directly.
2.  **Access images with code:** You can fetch the images using the `links.json` file (see JavaScript example below).
3.  **Add images:**
    *   Upload your images to the `images` folder.
    *   Update `links.json` with image information (URL, source, etc.).
    *   Make a pull request (see [Contributing])!
## Using `links.json` (JavaScript Example)

```javascript
const axios = require('axios');

axios.get('https://raw.githubusercontent.com/rynxzyy/blue-archive-r-img/refs/heads/main/links.json')
  .then(response => {
    const imageData = response.data;
    imageData.forEach(item => {
      console.log("URL:", item);
    });
  })
  .catch(error => {
    console.error("Error fetching image URLs:", error);
  });
```

## Contributing

Feel free to contribute! The more images, the merrier. Please make sure the images are:

*  Related to Blue Archive (official art or fan art).
*  Decent quality. (Images should be clear and not blurry or pixelated.)

## License

All images belong to their respective creators and publishers. This repository is just for non-commercial fun.
