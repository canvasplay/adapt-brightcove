adapt-brightcove
===============================

A Presentation component allowing Brightcove videos to be embedded natively in Adapt by using the Brightcove APIs to control and track video playback.

## Usage

Login to your Brightcove account to retrieve your IDs.


### _accountId

(String) Your account ID. **Note** if uploading to an authoring tool, I recommend adding your organizations account ID as a default attribute to save time for content developers.

### _videoId

(String) The video ID.

### _videoPlayer

(String) The video player (video skin) you want to use. use `_default` for the Brightcove default.

### _audioPlayer

(Object) An optional attribute if you wish to use Brightcove for audio only content.

    _isEnabled

    (boolean) Default is false. Enables the audio player.

    _posterImage

    (String, optional) A link to a poster image that you wish to use. If this attribute is left empty will use the minimalist player, which just shows the controls bar.

### _transcript

(object) This is identical to the media component's transcript. Used [here](https://github.com/adaptlearning/adapt-contrib-media/#settings-overview)

## Limitations

*   Multiple _audioPlayer used within the same course don't work. Just stick to one.
*   Unlike the Media component, if you have multiple instances of this component on a page. Playing one won't pause another already in play.

---

Version number: 1.5.0
Framework versions: ^2.0.0
Maintainer: <a href='mailto:simon.date@kcl.ac.uk'>Simon Date</a>
