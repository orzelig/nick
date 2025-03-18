# Nick DiGiovanni - Kid-Friendly Videos

A static webpage showcasing kid-friendly cooking videos from Nick DiGiovanni's YouTube channel.

## Features

- Responsive grid layout
- Mobile-friendly design
- Kid-friendly video selection
- Easy to maintain and update

## Setup

1. Fork this repository
2. Clone your forked repository
3. Edit the `index.html` file to add or modify videos
4. Commit and push your changes

## Adding Videos

To add a new video:

1. Find the video ID from the YouTube URL (e.g., for `https://www.youtube.com/watch?v=abc123xyz`, the ID is `abc123xyz`)
2. Add a new video item in the `video-grid` section of `index.html`:

```html
<div class="video-item">
    <div class="video-container">
        <iframe src="https://www.youtube.com/embed/VIDEO_ID" 
                title="Nick DiGiovanni Cooking Video" 
                frameborder="0" 
                allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
                allowfullscreen></iframe>
    </div>
    <div class="video-title">Video Title</div>
</div>
```

## Deploying to GitHub Pages

1. Go to your repository's Settings
2. Scroll down to the "GitHub Pages" section
3. Under "Source", select the branch you want to deploy (usually `main` or `master`)
4. Click "Save"

Your site will be available at `https://[your-username].github.io/[repository-name]`

## Contributing

Feel free to submit issues and enhancement requests!

## License

This project is licensed under the MIT License - see the LICENSE file for details. 