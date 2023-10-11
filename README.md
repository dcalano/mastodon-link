# Mastodon Linker Chrome Extension (Augmented)

Augmented version of the original Mastodon Linker extension by `@indiealexh`. I don't really need a user profile to take me to my home instance in order to follow them. Instead, I have updated the code so that it will take me to the target user's profile page on their own home instance. This way I can view more of their posts.

Unfortunately, after tinkering around with this, I have realized that it will only work in selective circumstances, such as when viewing a user's profile page on any server. Status updates will display the updated icon href link next to the user's `@id@instance` name header correctly but it is not clickable as one of the parent div containers overlays the link text. The link for this overlay can be removed but when testing this I found out that Mastodon is unfortunately hijacking the clicks anyway in order to run some navigation code that dynamically takes me to the exact place I was trying to avoid.

Still looking into how to get around that, but for now it's a slightly better Mastodon user experience coupled with the Graze extension.

## Build

- `npm install`
- `npm run build`
- You can then load the extension from the `dist` directory

## Installation

### Chrome
- Install it from [the Chrome Web Store](https://chrome.google.com/webstore/detail/mastodon-link/nlfdgcdfjnobjocicnddjghdbmgglame)
- Git clone this repo and [load it unpacked](https://developer.chrome.com/docs/extensions/mv3/getstarted/development-basics/#load-unpacked)

## Setup

Click on the mastodon link chrome extensions options:

<img width="317" alt="mastodon-link-options" src="https://user-images.githubusercontent.com/1066212/203490862-0e62fe47-1f74-41b3-99a8-4de640847d8c.png">

Enter your instances hostname and click save:

<img width="359" alt="mastodon-link-options-setup" src="https://user-images.githubusercontent.com/1066212/203490871-566cd1fc-a4b4-4ef6-a7c8-1f1c4769c04d.png">

Find a mastodon username and enjoy the convenient icon link!

![-indiealexh-tny-social-indiealexh-Twitter](https://user-images.githubusercontent.com/1066212/203491063-f5025516-e172-4838-a11a-55a5e5a1707d.png)

## License

This project is released under the Unlicense license. See the enclosed LICENSE for details.
