![logo](https://raw.githubusercontent.com/kochd/electricsheep-hd-client/master/logo.png)
# electricsheep-hd-client
[Wikipedia](https://en.wikipedia.org/wiki/Electric_sheep):
`Electric Sheep is a distributed computing project for animating and evolving fractal flames, which are in turn distributed to the networked computers`

Originally designed by pioneer [Scott Draves](https://github.com/scottdraves/electricsheep.git) and presented on [website](http://www.electricsheep.org/), rendering runs with resolutions from last century.
Hosted by and thanks to [kochd's codes,](https://github.com/kochd/electricsheep-hd-client/master/) are actual electric dreaming sheeps further fulfilled with
HighDef' graphical participactive works ran by 'electricsheep-hd-client' daemons, synchronized all together to generate new High-Definition electric sheep dreams frames.
(fitting HD displays standards up to 720p, 1080p, 4k, 8k)
For a good illustration of electric sheeps, you might have a look to [this youtube video](https://www.youtube.com/watch?v=KeNORUW4OGs)

### Road map
- not set.

## Getting started
### To run it on [Debian-based](https://github.com/alidruno/electricsheep-hd-client/blob/master/README.md#debian--ubuntu--) distributions as Ubuntu (which I mostely run)...
it is done with this command-lines:

<pre>
git clone https://github.com/alidruno/electricsheep-hd-client.git && cd electricsheep-hd-client
sudo apt-get install flam3-utils flam3-palette libflam3-0 ruby3.0 bundler -y
bundle install
./daemon
</pre>

### For other Linux / Unix / Posix system users,
you should try successfully with usual methods and relate-back their experiences through welcomed contributions what might enhance the discovery of this project as they should climb up back to original code writers having made it ready and free to share.

If message  `./daemon.rb:29:in <main>': You will need an api key. Please register at https://sheeps.triple6.org:9999/register (RuntimeError)`  is displayed,
everything invites you to [register](https://sheeps.triple6.org:9999/register) on this page.

### With Windows,
Just download and run the [latest release](https://github.com/alidruno/electricsheep-hd-client/releases/latest) installer and follow the registration steps to get your apikey.
If you want the latest development version, use the same installer file and replace every existing file in the installation folder with the content of the [latest master](https://github.com/alidruno/electricsheep-hd-client/archive/master.zip). This usually isn't needed as new installers are packaged at same time.

### Registration
Is taking place on this [page](https://sheeps.triple6.org/register), then, follow the instructions received by email.

### Warning because
Website's SSL certificate is self-signed and shouldn't, regardless the warning, put you at risk nor prevent you getting the needed api.key.

### Man electricsheep-hd-client
<pre>
Usage: daemon [OPTIONS]
        --apikey APIKEY              Your api key is read by default from ./api.key file
        --debug                      Debug-mode
        --gpu                        Use GPU renderer (Fractorium - http://fractorium.com/)
        --gpu-devices [Device-Ids]   Use device(s) with given ids e.g.: '2,3'. Use --gpu-list-devices to get a list of your available devices.
        --gpu-list-devices           Returns a list of your installed OpenCL devices
        --gpu-priority               Set GPU render priority (1: lowest, 99: highest)
        --help                       Shows you this updated man page
        --insecure                   Ignore ssl certificate errors
    -k, --keep-frames                Do not delete rendered frames after upload
        --nd, --no-download          Will let the daemon render without asking for new movies
        --np, --no-progress          Without shown progress and ETA to compute, a bit more goes to rendering
        --nice NICENESS              Niceness (Higher values result in lower process priority (default: 19, min:-20, max: 19))
        --server SERVER              Control server to connect to
</pre>
(This list might be outdated. Use --help option to check which are really available)

Once your daemon is rendering frames, you will earn so called credits for every rendered frames. Your daemon will then start to exchange them, harvesting answered electricsheep-hd videos sequences (if  --no-download  option is not set). Downloaded movies are stored in `$BASE_DIR/branches/$CURRENT_BRANCH/movies` directory. Currently you will only get ~5 seconds long sequences allowing the play script to display them immediately.

### Play
Just run
<pre>
./play
</pre>

This should read your accumulated movies from the current season to play them using mpv (https://mpv.io). mpv is also available as apt package and included in the windows installer.

### Setups
Have a look at the README's in [setups](https://github.com/alidruno/electricsheep-hd-client/tree/master/setups) to find pretty huge and well prepared advanced setups, fitting your client in very easy-going few steps up to the best integration.

#### More information can be found on following links
- [FAQ](https://sheeps.triple6.org/faq)
- [Wiki](https://github.com/kochd/electricsheep-hd-client/wiki/Season)
- [Feel free to submit any questions to the honorific source teams](https://github.com/kochd/electricsheep-hd-client/issues/new?labels=question)
- I am surely not able to make better answer as them.
