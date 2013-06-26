
# HOW-TO Install Style

1.  Install font **Open Sans Light** http://opensans.com/

2. First install **Conky** if you don't have it, Slackware:

  `# sbokpkg -i "scons lua imlib2 tolua++ conky"`

3. Extract contents of the archive into your home folder

4. Open the file `.conkyrc` with a text editor and:

  Search for `gap_x` (conky setting) and replace it with your own display width. Follow this formula: `gap_x = display_width - 255px`

  Search for **346058** and replace it with the **WOEID** of your own location. To find your WOEID, browse or search for your city from the Yahoo Weather home page http://weather.yahoo.com/. The WOEID is in the URL for the forecast page for that city.

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
