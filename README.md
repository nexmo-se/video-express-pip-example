# Video Express PiP Example

This application shows how to use (Vonage Video Express SDK)[https://tokbox.com/developer/video-express/] for a Picture in Picture use case.

## Instructions

1. Run `npm install`
2. Run `npm start`

## How it works

The relevant code is on the room init method, `managedLayoutOptions` --> `cameraPublisherContainer`:

```
const room = new VideoExpress.Room({
    apiKey: '', // add your OpenTok API key
    sessionId: '', // add your OpenTok Session ID
    token: '', // add your OpenTok token
    roomContainer: 'roomContainer',
    managedLayoutOptions: {
        cameraPublisherContainer: 'publisher-video-container'
    }
});
```

The `publisher-video-container` is a div with `position:absolute` at the bottom right of the page. You can edit this behaviour on the `css/index.css` file.
