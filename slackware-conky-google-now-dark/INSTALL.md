
# HOW-TO Install Style

1. Install font **Open Sans Light** http://www.opensans.com/

  Slackware:

  `$ git clone https://github.com/51114u9/slackbuilds.git`

  `$ cd slackbuilds/graphics/opensans-ttf`

  `$ su`

  `# sh ./opensans-ttf.SlackBuild --cleanup`

  `# upgradepkg --install-new /tmp/opensans-*.t?z`

2. Install **conky requirements** if you don't have it

  Slackware:

  `# sbokpkg -i "scons lua imlib2 tolua++ conky"`

3. Extract contents of the archive into your home folder

  `$ unzip conky-theme-master.zip`

  `$ cd conky-themes-master/slackware-conky-google-now-dark`

  `$ mkdir -p ~/.cache/conky`

  `$ install -m 600 .conkyrc ~/`

  `$ cp -R .config ~/`

4. Open the config file `.conkyrc` with your favorite text editor and:

  Find `gap_x` and replace it with your own display width. Follow this formula: `gap_x = display_width - 254`

  Find `346058` and replace it with the **WOEID** of your own location. *To find your WOEID, browse or search for your city from the Yahoo Weather home page http://weather.yahoo.com/. The WOEID is in the URL for the forecast page for that city*

  Find *System info** section and customize with your own file system layout

5. Add "Conky" to your **Startup Applications**:

  XFCE:

    >XFCE Config > Session & Start > Auto-Start
    >
    >**Name**: Conky
    >
    >**Description**: A system monitor for X
    >
    >**Command**: `sleep 5 && conky -d`

6. Enjoy!

B^)
