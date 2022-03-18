<h1>Dotfiles</h1>

These are all my Dotfiles so far, i will update them as i change them.<br/>
\! All the changes to the original files are listed in each section so you can modify only those lines without downloading and replacing the whole file.<br/>
\! All the screenshots are taken with a custom <a href="palette">palette</a>, final results may vary from the images shown here.
<h2>Index</h2>
<ul>
  <li><a href="prompt">Prompt</a></li>
  <li><a href="dircolors">Dircolors</a></li>
  <li><a href="conkyrc">Conky</a></li>
  <li><a href="glava">Glava</a>
    <ul>
      <li><a href="bars">Bars</a></li>
      <li><a href="rc">Rc</a></li>
    </ul>
  </li>
  <li><a href="neofetch">Neofetch</a></li>
  <li><a href="ranger">Ranger</a>
    <ul>
      <li><a href="theme">Theme</a></li>
      <li><a href="rrc">Rc</a></li>
      <li><a href="rifle">Rifle</a></li>
      <li><a href="scope">Scope</a></li>
    </ul>
  </li>
  <li><a href="terminals">Terminals</a>
    <ul>
      <li><a href="coolterm">Coolterm</a></li>
      <li><a href="alacritty">Alacritty</a></li>
    </ul>
  </li>
  <li><a href="kwin">Kwin</a></li>
  <li><a href="logicd">Logiops</a></li>
  <li><a href="touchegg">Touchegg</a></li>
  
</ul>
<hr/><br/><br/>
<h2 id="prompt">Prompt</h2>
![image](https://user-images.githubusercontent.com/81905574/159064860-d8cb1368-94f3-4d8e-b276-b2a206b515df.png)<br/>
This prompt is made for the zsh shell, to use it add it to your .zshrc file or if you are using <a href="">Oh-my-Zsh!</a> create a theme in `/usr/share/ohtmyzsh/themes` named like _mytheme.zsh-theme_
and change the _ZSH_THEME_ to the name of your theme (without file extension).

<h2 id="dircolors">Dircolors</h2>
![image](https://user-images.githubusercontent.com/81905574/159063606-d835d776-49ba-4988-9dd5-1c9d66dd2663.png)<br/>
To use this dircolors you have to set up in your bashrc/zshrc/kshrc a line like this one:<br/>
`eval $(dircolors /location/of/dircolors/file)`
<h2 id="conkyrc">Conky</h2>
<br/>
This is the output of the .conkyrc file, to change the accent color modify _default_color_ in .conkyrc and set it to your desired color,
the location is set for a 1920x1080p screen, adjust it to your screen values.

<h2 id="glava">Glava</h2>
<br/>
In my case the glava size and position is adjusted to fit on top of the conky window.
  <h3 id="bars">Bars</h3>
    
      
  <h3 id="rc">Rc</h3>
 
<h2 id="neofetch">Neofetch</h2>
![image](https://user-images.githubusercontent.com/81905574/159067790-b97564b8-b93b-4945-9442-0f8370d528d9.png)<br/>
All the colors are from an <a href="https://misc.flogisoft.com/_media/bash/colors_format/256_colors_bg.png">ansi color table</a> (Image from Flozz' MISC)

<h2 id="ranger">Ranger</h2>
  
  <h3 id="theme">Theme</h3>
    
  <h3 id="rrc">Rc</h3>
    
  <h3 id="rifle">Rifle</h3>
    
  <h3 id="scope">Scope</h3>

<h2 id="terminals">Terminals</h2>
  <h3 id="alacritty">Alacritty</h3>
  ![image](https://user-images.githubusercontent.com/81905574/159072300-f885bbca-6a7d-4694-93de-2208d8d497f1.png)
  <h3 id="coolterm">Cool Retro Term</h3>
  ![image](https://user-images.githubusercontent.com/81905574/159072884-4742c41e-a0ae-4833-bfe2-ee77928bf14a.png)
  (To much bloom, i know, but this terminal it's just for flexing not for work)

<h2 id="kwin">Kwin</h2>
  
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
