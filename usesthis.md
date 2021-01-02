# Uses This
I really enjoy to read posts about the tools/setup/workplace from other people like on [usesthis.com](https://usesthis.com/). So here is mine.

## Links to others I found intresting
- [Scott Hanselmann's Ultimate Developer and Power Users Tool List for Windows](https://www.hanselman.com/blog/scott-hanselmans-2021-ultimate-developer-and-power-users-tool-list-for-windows)
- [Michael Staperberg's uses this: my 2020 desk setup](https://michael.stapelberg.ch/posts/2020-05-23-desk-setup/)
- [Håkon Wium Lie on usesthis.com](https://usesthis.com/interviews/hakon.wium.lie/)
- [Stephen Wolfram's Seeking the Productive Life: Some Details of My Personal Infrastructure](https://writings.stephenwolfram.com/2019/02/seeking-the-productive-life-some-details-of-my-personal-infrastructure/)

## Hardware
### Home
- [Google Pixel 4a](https://store.google.com/product/pixel_4a) as my smartphone.
- [Lenovo ThinkCentre M93p Tiny Intel i3-4130T, 4GB RAM, 320 GB HDD](https://support.lenovo.com/de/de/solutions/pd027573-detailed-specifications-for-thinkcentre-m93-m93p-tiny-form-factor) as home server. It use 11 Watt per hour which is low enough with around 0.30 Euro Cent per kWh costs in Germany. 
- [Mac Mini Late 2009](https://everymac.com/systems/apple/mac_mini/specs/mac-mini-core-2-duo-2.53-late-2009-specs.html) as my desktop machine with 4GB RAM. It has two external hard drives for data and Time Machine backups. The last available Mac OS X version is 10.11.6 (El Capitan) and I'm okay with it. Recently I had to switch my mail client because Apple Mail can't handle TLS 1.2 in this version
- [Dell P2415Q 4K Monitor](https://www.dell.com/de-de/work/shop/cty/pdp/spd/dell-p2415q-monitor) connected via HDMI with 1080p and it's okay. I use this monitor also when working from home in 4k resolution.
- As input devices I use a [Apple Magic Mouse](https://en.wikipedia.org/wiki/Magic_Mouse) or a [Evoluent Vertical Mouse 4](https://evoluent.com/products/vm4r/) and [Happy Hacking Keyboard Lite 2](https://deskthority.net/wiki/HHKB_Lite) or a [BTC 5100C](http://deskthority.net/wiki/BTC_5100). The HHKB Lite is about 10 years old and was before in use at work and it doesn't fill any good to type on it anymore. Now mostly I use the BTC 5100C and I really like it.
- [iPad Air Wi-Fi](https://everymac.com/systems/apple/ipad/specs/apple-ipad-air-1st-gen-a1474-wi-fi-only-specs.html) still in iOS 12 but I only used it for reading and connecting to my home server via SSH with a [Logitech K380](https://support.logi.com/hc/en-us/articles/360051435873-Getting-Started-K380-Multi-Device-Bluetooth-Keyboard-for-Mac) keyboard.
- Internet connection is a VDSL 50/10 Mbit/s. I connect to it with a [Daytrek Vigor 130](https://www.draytek.de/vigor130.html) in pass through mode to a [Ubiquiti EdgeRouter Lite](https://www.ui.com/edgemax/edgerouter-lite/). In a few month the new fiber optical connection will be available at my home and I can remove the VDSL modem. I hope I can also replace the ONT from the provider with the right GPON SFP directly in my router.
- The home network consist of two [Mikrotik RB2600GSP (CSS106-1G-4P-1S)](https://mikrotik.com/product/RB260GSP) switches which connect to each other via Single Mode fiber and SFP BiDi modules. It's much thinner cable and for me much easier to lay. I got inspired by [Michael Stapelberg's "Adding a fiber link to my home network"](https://michael.stapelberg.ch/posts/2020-08-09-fiber-link-home-network/) and [FS.com](https://www.fs.com/) is a great shop. I have also two Access Points [Mirkotik cAP ac](https://mikrotik.com/product/cap_ac) and [Mirkotik cAP lite](https://mikrotik.com/product/RBcAPL-2nD-307).

### Work
- Some recent 14 inch DELL Laptop
- [Jabra Evolve 75](https://www.jabra.com/business/office-headsets/jabra-evolve/jabra-evolve-75) headset
- [Vortex New 75 (Race 3) Model VTG-8200](http://www.vortexgear.tw/vortex2_2.asp?kind=47&kind2=225&kind3=&kind4=1044) with Cherry MX Brown switches as my keyboard. I like the form factor without a numpad so the movement to the mouse isn't to much and also the possibility to program it so I can remap the Caps Lock and Control keys without changing any settings in my operating system.
- [Evoluent Vertical Mouse 4](https://evoluent.com/products/vm4r/)

## Software
### Home
- I have created a chat bot with Python and [slixmpp](https://slixmpp.readthedocs.io/) which send me every morning the outside temperature, can dim my Hue lights, track my expense and more.
- I replaced grep with [rg](https://github.com/BurntSushi/ripgrep) and ls with [exa](https://github.com/ogham/exa) and love it.
- Backups are made with [restic](https://restic.net/) to [Backblaze B2](https://www.backblaze.com/)
- For bank stuff I use the fantastic [MoneyMoney](https://moneymoney-app.com/) (one of the reasons I still use the old Mac Mini). It can connect also to PayPal and import transaction from csv files which I fill with my chat bot.
- My text editor of choice is [Vim](https://www.vim.org/). I don't use any plugins and very basic config. Most used features are Macros for massive one shot manipulation of text data for preparation to import into Excel.
- I use [Syncthing](https://en.wikipedia.org/wiki/Bitstream_Vera) to sync my document folder between my Mac Mini, home server and smartphone.
- On my home server I run RSS reader [Miniflux](https://en.wikipedia.org/wiki/Bitstream_Vera) with [rss-bridge](https://github.com/RSS-Bridge/rss-bridge/) to integrate some Twitter and Facebook accounts and for our local newspaper which just doesn't provide a rss feed. I save interesting links to things posted on webpages as text file and review it later, if it worth reading for me. If I would like to read it, I make a PDF or epub (with [dotepub](https://uniballco.com/kuru-toga-elite/)) of the link and import it to my calibre database. With [Calibre-Web](https://github.com/janeczku/calibre-web) I can access my calibre database from my devices easily.
- After TLS 1.2 only switch of my mail provider [mailbox.org](https://www.mailbox.org) I have switched to [mutt](http://www.mutt.org/) with [offlineimap](https://www.offlineimap.org/), [fdm](https://github.com/nicm/fdm) for POP3-Accounts, [notmuch](https://notmuchmail.org/) for searching and [khard](https://github.com/scheibler/khard/) and [vdirsyncer](https://github.com/pimutils/vdirsyncer) for addresses. This all runs on my home server which I can access via SSH. Setup with the great documentation from the [Arch Linux Wiki](https://wiki.archlinux.org/index.php/Mutt).
- [tmux](https://github.com/tmux/tmux) as my terminal multiplexer.
- My printer is a Epson ET-2650 with ink tanks.
- My browser since years is [Mozilla Firefox](https://www.mozilla.org/en-US/firefox/new/) also on my smartphone with Firefox Sync service.
- On my smartphone I use [K9-Mail](https://k9mail.app/), [Opentasks](https://opentasks.app/), [Etar](https://github.com/Etar-Group/Etar-Calendar), [KeePassDX](https://www.keepassdx.com/), [Total Commander](https://www.ghisler.com/), [Conversation](https://conversations.im/), [WhatsApp](https://www.whatsapp.com/), [Spotify](https://www.spotify.com/), [meteoblue](https://play.google.com/store/apps/details?id=com.meteoblue.droid&utm_source=Website&utm_campaign=Permanent), [Firefox](https://www.mozilla.org/en-US/firefox/mobile/), [Book Read](https://play.google.com/store/apps/details?id=com.github.axet.bookreader&hl=en_US&gl=US), [Corona-Warn](https://www.coronawarn.app/), [ICSx5](https://icsx5.bitfire.at/) and [DAVx5](https://www.davx5.com/), [Markor](https://github.com/gsantner/markor), [Syncthing](https://syncthing.net/), [MuPDF Mini](https://mupdf.com/), [Telegram](https://telegram.org/), [WarnWetter](https://www.warnwetterapp.de/), [WiFiAnalyzer](https://play.google.com/store/apps/details?id=com.vrem.wifianalyzer&hl=de&gl=US)
- My preferred font in terminal sessions is [Bitstream Vera Sans Mono](https://en.wikipedia.org/wiki/Bitstream_Vera).

### Work
- Windows 10 with Office 365 and a lot of Excel (e.g. my to do list).
- [SecureCRT](https://www.vandyke.com/products/securecrt/) as SSH and since 9.0 RDP client which a tone of handy features.
- [rg](https://github.com/BurntSushi/ripgrep) for searching through big log files.
- [Total Commander](https://www.ghisler.com/) for all file system stuff.
- My browser is [Microsoft Edge](https://www.microsoft.com/en-US/edge), the new one based on chromium.
- [Ditto](https://ditto-cp.sourceforge.io/) as clipboard manager and [Claiver+](https://gryder.org/software/clavier-plus/?lang=en) as text expander much improved my efficiency. Never think again, if I can copy this to the clipboard and lost the previous content or be annoyed by typing again my email address (40 characters!).
- [Greenshot](https://getgreenshot.org/) for screenshots and quick image manipulations.
- [Tomighty](https://tomighty.github.io/) for breaks and more structure.
- I prefer a [Leuchtturm 1917](https://www.leuchtturm1917.de) paper notebook classic in A5 dotted and love my [uni-ball Kuru Toga Elite](https://uniballco.com/kuru-toga-elite/) mechanical pencil.

## Future Ideas
I really like to have a treadmill setup like Stephen Wolfram.

## Contact
If you want to make a comment or have a question just write me an email jummo(at)mailbox.org.

--
January 2021
