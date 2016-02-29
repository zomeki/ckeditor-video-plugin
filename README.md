# ckeditor-video-plugin

Plugin video for CKEditor

Original work:
 - http://ckeditor.com/forums/Plugins/HTML5-Video
 - http://alfonsoml.blogspot.fr/2011/01/html5-video-plugin-for-ckeditor.html
 - https://dmlogic.com/

I just added the OGG input fields.

## Integration with CKEditor

### Normal

see [docs/install.html](docs/install.html)

### Symfony

With https://github.com/trsteel88/TrsteelCkeditorBundle

```yml
# app/config/config.yml

trsteel_ckeditor:
    transformers: [] # you can tune here
    toolbar_groups:
        styles: [ ..., 'Video', ... ]
    extra_allowed_content: "video source [*]"
    external_plugins:
            video:
                path: js/ckeditor/plugins/video

# dont' forget the filebrowser_browse_url, ... 
                
```
