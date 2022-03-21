<h1>Dotfiles</h1>
<image src="https://user-images.githubusercontent.com/81905574/159300636-181fe55e-9723-4341-821b-f9c6c13885c5.png">
These are all my Dotfiles so far, i will update them as i change them.<br/>
! All the changes to the original files are listed in each section so you can modify only those lines without downloading and replacing the whole file.<br/>
! All the screenshots are taken with a custom <a href="palette">palette</a>, final results may vary from the images shown here.
<h2>Index</h2>
<ul>
  <li><a href="#prompt">Prompt</a></li>
  <li><a href="#dircolors">Dircolors</a></li>
  <li><a href="#conkyrc">Conky</a></li>
  <li><a href="#glava">Glava</a>
    <ul>
      <li><a href="#bars">Bars</a></li>
      <li><a href="#rc">Rc</a></li>
    </ul>
  </li>
  <li><a href="#neofetch">Neofetch</a></li>
  <li><a href="#ranger">Ranger</a>
    <ul>
      <li><a href="#theme">Theme</a></li>
      <li><a href="#rrc">Rc</a></li>
      <li><a href="#rifle">Rifle</a></li>
      <li><a href="#scope">Scope</a></li>
    </ul>
  </li>
  <li><a href="#terminals">Terminals</a>
    <ul>
      <li><a href="#colors">Palette</a></li>
      <li><a href="#coolterm">Coolterm</a></li>
      <li><a href="#alacritty">Alacritty</a></li>
    </ul>
  </li>
  <li><a href="#kwin">Kwin</a></li>
  <li><a href="#logicd">Logiops</a></li>
  <li><a href="#touchegg">Touchegg</a></li>
  <li><a href="#repos">App repos</a></li>
</ul>

<hr/><br/><br/>
<h2 id="prompt">Prompt</h2>
<img src="https://user-images.githubusercontent.com/81905574/159064860-d8cb1368-94f3-4d8e-b276-b2a206b515df.png">
This prompt is made for the zsh shell, to use it add it to your .zshrc file or if you are using <a href="">Oh-my-Zsh!</a> create a theme in <code>/usr/share/ohtmyzsh/themes</code> named like _mytheme.zsh-theme_
and change the <i>ZSH_THEME</i> to the name of your theme (without file extension).

<h2 id="dircolors">Dircolors</h2>
<img src="https://user-images.githubusercontent.com/81905574/159063606-d835d776-49ba-4988-9dd5-1c9d66dd2663.png">
To use this dircolors you have to set up in your bashrc/zshrc/kshrc a line like this one:<br/>
<code>eval $(dircolors /location/of/dircolors/file)</code>
<h2 id="conkyrc">Conky</h2>
<img width="300px" src="https://user-images.githubusercontent.com/81905574/159129032-243233e8-8748-41c1-a3c0-bbb7e2c56e75.gif">
This is the output of the .conkyrc file, to change the accent color modify <i>default_color</i> in .conkyrc and set it to your desired color,
the location is set for a 1920x1080p screen, adjust it to your screen values.
<h2 id="glava">Glava</h2>
<img width="300px" src="https://user-images.githubusercontent.com/81905574/159129047-39effc96-ca6b-4554-adc1-8fba6a8a5395.gif">
In my case the glava size and position is adjusted to fit on top of the conky window.
  <h3 id="bars">bars.glsl</h3>
    <pre><code>
     BAR_WIDTH 8
     BAR_GAP 2
     BAR_WIDTH 0
     GRADIENT_POWER 100
     GRADIENT (d / GRADIENT_POWER + 0.1)
     COLOR (#cf0000 * GRADIENT)
     </code></pre>
  <h3 id="rc">rc.glsl</h3>
     <pre><code>
      setdecorated false
      setmirror true
      setgeometry 1490 -390 435 600
      setxwintype "dock"
      addxwinstate "below"
      addxwinstate "sticky"
      addxwinstate "skip_taskbar"
      addxwinstate "skip_pager"
      addxwinstate "pinned"
      setframerate 60
      setfullscreencheck true
      setprintframes false
      setforcegeometry true
     </code></pre>
<h2 id="neofetch">Neofetch</h2>
<img width="500px" src="https://user-images.githubusercontent.com/81905574/159067790-b97564b8-b93b-4945-9442-0f8370d528d9.png">
All the colors are from an <a href="https://misc.flogisoft.com/_media/bash/colors_format/256_colors_bg.png">ansi color table</a> (Image from Flozz' MISC)

<h2 id="ranger">Ranger</h2>
  <h3 id="theme">theme.py</h3>
    To apply the theme you have to type this commands:
    <code>mkdir ~/.config/ranger/colorschemes && mv <theme>.py ~/.config/ranger/colorschemes</code>
    And edit the colorscheme line to your preferences
  <h3 id="rrc">rc.conf</h3>
    <pre><code>
      preview_images true
      colorscheme <theme without the .py>
      collapse_preview false
      mouse_enabled false
    </code></pre>
  <h3 id="rifle">rifle.conf</h3>
    These lines aren't modified, you have to add them
    <pre><code>
       !mime ^text, label editor. has atom, ext xml|json|csv|tex|py|pl|rb|js|sh|php = atom -- "$@" & disown
       !mime ^text, label pager. has highlight, ext xml|json|csv|tex|py|pl|rb|js|sh|php = highlight -O ansi | less -- "$@"
    </code></pre>
  <h3 id="scope">scope.sh</h3>
    <pre><code>
      PYGMENTIZE_STYLE="${PYGMENTIZE_STYLE:-monokai}"
    </code></pre>
    
<h2 id="terminals">Terminals</h2>
  <h3 id="colors">Color palette</h3>
  <pre>
    -Normal colors            -Bright colors
    black:   0x000000         black:   0x585858
    red:     0xc92c2c         red:     0xd44646
    green:   0x7dcf3e         green:   0xa1b56c
    yellow:  0xcfcf3e         yellow:  0xf7ca88
    blue:    0x3e82cf         blue:    0x7cafc2
    magenta: 0xad51b5         magenta: 0xba8baf
    cyan:    0x51b5a1         cyan:    0x86c1b9
    white:   0xd8d8d8         white:   0xf8f8f8
  </pre>
  <h3 id="alacritty">Alacritty</h3>
  <img width="500px" src="https://user-images.githubusercontent.com/81905574/159072300-f885bbca-6a7d-4694-93de-2208d8d497f1.png">
  <h3 id="coolterm">Cool Retro Term</h3>
  <img width="500px" src="https://user-images.githubusercontent.com/81905574/159072884-4742c41e-a0ae-4833-bfe2-ee77928bf14a.png">
  (To much bloom, i know, but this terminal it's just for flexing not for work)

<h2 id="kwin">Kwin</h2>
  <img src="https://user-images.githubusercontent.com/81905574/159296759-32d9197b-04e2-45b0-bf01-3f0379686fa1.png">
  The blur effect is achieved with this <a href="https://github.com/esjeon/kwin-forceblur">kwin script</a> from <a href="https://github.com/esjeon">esjeon</a><br/>
  These are the apps that i dont want to make translucent, if you want to add more all you have to do is append to the opaque section like this:</br>
  <code>wmclass=firefox|atom|kate|virtualbox|newapp1|newapp2</code><br/>
 Opaque apps:
  <ul>
    <li>Firefox</li>
    <li>Atom</li>
    <li>Kate</li>
    <li>Virtualbox</li>
  </ul>
<h2 id="logicd">Logiops</h2>
  These are all my gestures for the MX Master 3:
    <ul>
      <li>Thumb button
        <ul>
           <li>Drag left -> Move window to left</li>
           <li>Drag right -> Move window to right</li>
           <li>Drag up -> Maximize window</li>
           <li>Drag down -> Minimize window</li>
        </ul>
      </li>
      <li>Thumb wheel
        <ul>
           <li>Tap -> Alt key</li>
           <li>Scroll up -> Next app</li>
          <li>Scroll down -> Previous app</li>
        </ul>
      </li>
      <li>Central button
          <ul>
           <li>Click -> Lock/Unlock wheel</li>
           <li>Drag right -> Previous desktop</li>
           <li>Drag left -> Next desktop</li>
           <li>Drag down -> Close session</li>
        </ul>
      </li>
    </ul>
<h2 id="touchegg">Touchegg</h2>
   <ul>
    <li>Two fingers
       <ul>
         <li>Drag up/down -> Scroll vertically</li>
         <li>Drag right/left -> Scroll horizontally</li>
       </ul>
    </li>
    <li>Three fingers
      <ul>
         <li>Drag up -> Maximize window</li>
         <li>Drag down -> Minimize window</li>
         <li>Drag right/left -> Scroll through runnning apps</li>
       </ul>
    </li>
    <li>Four fingers
        <ul>
         <li>Drag down -> Show desktop</li>
         <li>Drag right -> Previous desktop</li>
         <li>Drag left -> Next desktop</li>
       </ul>
    </li>
   </ul>
  <h1 id="repos">Repos of all the apps used</h1>
      Im not the owner of any app listed here, all rights reserved to their creators.
      <ul>
        <li><a href="https://github.com/ohmyzsh/ohmyzsh">OhMyZsh!</a></li>
        <li><a href="https://github.com/ranger/ranger">Ranger</a></li>
        <li><a href="https://github.com/Swordfish90/cool-retro-term">Cool Retro Term</a></li>
        <li><a href="https://github.com/brndnmtthws/conky">Conky</a></li>
        <li><a href="https://github.com/jarcode-foss/glava">Glava</a></li>
        <li><a href="https://github.com/dylanaraps/neofetch">Neofetch</a></li>
        <li><a href="https://github.com/abishekvashok/cmatrix">Cmatrix</a></li>
        <li><a href="https://github.com/JoseExposito/touchegg">Touchegg</a></li>
        <li><a href="https://github.com/PixlOne/logiops/">Logiops</a></li>
      </ul>
