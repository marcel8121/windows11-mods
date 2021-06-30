<!DOCTYPE html>
<html>
<body>
<img align="center" src="https://i.pcmag.com/imagery/articles/07byLBF5UaGsFsKtyOsENAg-11.1624559555.fit_lim.png">
<h1 align="center">
  <p>Windows 11 modifications</p>
</h1>

<p align="center">
  Windows 11 Preview is now available for insiders. There are a lot of great changes, but some features are annoying.
  </p>
  <p align="center">🔷NOTE that you are doing this at your own risk. Changing the wrong thing could lead to break your System.🔷</p>
<p align="center">
  <a href="#first">Do this first</a>
  •
  <a href="#taskbar_position">Taskbar position</a>
  •  
  <a href="#taskbar_size">Taskbar size</a>
  •
  <a href="#classic_menu">Old Startmenu</a>
</p>
#first
<p> 
<a id="#first">Do this first</a>                            
    This will be our friend throughout this Guide.
    You can do that by pressing Windows + R and type regedit
</p>
#taskbar_position
<a id="#taskbar_position">Taskbar position</a>
<p>1. Navigate to: <b>HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\StuckRects3</b></p> 
<p>You can copy and paste this in the search bar.</p>
<p>2. Doubleklick "Settings" in the right field.</p>
<p> 3. In the second row you will change the fifth value to:</p>
<table>
  <thead>
    <tr>
      <th>value</th>
      <th>position</th>
    </tr>
   </thead>
   <tbody>
     <tr>
       <td>00</td>
       <td>left</td>
     </tr>
     <tr>
       <td>01</td>
       <td>top</td>
     </tr>
     <tr>
       <td>02</td>
       <td>right</td>
     </tr>
     <tr>
       <td>03</td>
       <td>bottom</td>
     </tr>
  </tbody>
</table>
<p> Then restart explorer.exe or just restart the PC </p>
<p>
  <br>
  <img width="50%" src="https://raw.githubusercontent.com/marcel-kraatz/windows11-mods/main/StuckRects3.png">
  <img width="40%" src="https://raw.githubusercontent.com/marcel-kraatz/windows11-mods/main/stuckrects.png">
  <br>
</p>

<b>OPTIONAL</b>
<p>If you have multiple displays and multiple taskbars (why?) then you can change it here:</p>
<p>(4). <b>HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\MMStuckRects3</b></p>
<p>Repeat the Steps 3 and 4 for each value</p>
#taskbar_size
<a id="#taskbar_size">Taskbar size</a>
<p>1. Navigate to: <b>HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\</b></p>
<p>2. Do a quick leftklick in the right field select New -> DWORD-Value (32 bit)</p>
<p>3. Name this new value <b>TaskbarSi</b></p>
<p>4. Then double click the Value and change the value to:</p> 
<table>
  <thead>
    <tr>
      <th>value</th>
      <th>position</th>
    </tr>
   </thead>
   <tbody>
     <tr>
       <td>0</td>
       <td>small</td>
     </tr>
     <tr>
       <td>1</td>
       <td>medium</td>
     </tr>
     <tr>
       <td>2</td>
       <td>large</td>
     </tr>
  </tbody>
</table>
<p> Then restart explorer.exe or just restart the PC </p>
#classic_menu
<a id="#classic_menu">Old Startmenu</a>
<p>1. Navigate to: <b>HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced</b></p>
<p>2. Do a quick leftklick in the right field select New -> DWORD-Value (32 bit)</p>
<p>3. Name this value Start_ShowClassicMode and change the value to:</p>
<table>
<thead>
<tr>
<th>value</th>
<th>position</th>
</tr>
</thead>
    <tbody>
    <tr>
        <td>0</td>
        <td>New Windows 11 Menu</td>
    </tr>
    <tr>
        <td>1</td>
        <td>Good old Windows 10 Menu</td>
    </tr>
    </tbody>
</table>
<p>I prefer the old one because i have all my stuff there to keep my desktop clean</p>
<p>Then restart explorer.exe or just restart the PC</p>
   
  </body>
</html>
