# Spotify Embed Shortcode for micro.blog

This project provides a shortcode to easily embed Spotify tracks and albums in your micro.blog posts.

## Installation

To use this shortcode, you can install it from the [micro.blog](https://micro.blog) plugin directory.

## Configuration

Navigate to the settings of the plugin (Plugins on the sidebar, then settings next to this plugin) and you've a few options to play with:

- Top margin: Sets the CSS `margin-top` in `rem`. This defaults to 0.
- Bottom margin: Sets the CSS `margin-bottom` in `rem`. Default is 0.
- Height: Sets the vertical size of the embed. Can be `tall` or `compact`. Default is `compact`.
- Use colorful theme: Set to `true` for colorful theme, `false` for default spotify theme.


## Usage

To embed a Spotify track or album, simply use the Spotify share sheet to select a song or album and then use the following shortcode in your Hugo content files, replacing the URL with what you've copied:

```markdown
{{< spotify url="https://open.spotify.com/track/5vdEuDGGG5PuyHwN6xtc6W?si=0316b808513942d6" >}}
```

You can also override the default configuration by passing additional parameters:

- `url`: The Spotify URL of the track or album (required).
- `width`: The width of the embed. Default is `100%`.
- `margin-top`: Top margin in `rem`. Overrides the default configuration.
- `margin-bottom`: Bottom margin in `rem`. Overrides the default configuration.

Example usage with additional parameters:

```markdown
{{< spotify url="https://open.spotify.com/track/5vdEuDGGG5PuyHwN6xtc6W?si=0316b808513942d6" width="80%" margin-top="1" margin-bottom="1" >}}
```

## License

This project is licensed under the MIT License.