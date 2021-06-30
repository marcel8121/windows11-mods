<h1 align="center">
  <br>
  <img src="https://i.pcmag.com/imagery/articles/07byLBF5UaGsFsKtyOsENAg-11.1624559555.fit_lim.png">
  <br>
  Windows 11 modifications
  <br>
</h1>

<p align="center">
  Windows 11 Preview is now available for insiders. There are a lot of great changes, but some features are annoying.
  <br>
  **NOTE that you are doing this at your own risk. Changing the wrong thing could lead to break your System.**
</p>

<p align="center">
  <a href="#First">Do this first</a>
  •
  <a href="#Taskbar_position">Taskbar position</a>
  •  
  <a href="#Taskbar_size">Taskbar size</a>
  •
  <a href="#Classic_menu">Old Startmenu</a>
</p>
 
# First                            

This will be our friend throughout this Guide.
You can do that by pressing Windows + R and type regedit

# Taskbar_position

1. Navigate to: HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\StuckRects3
    You can copy and paste this in the search bar.  

2. Doubleklick "Settings" in the right field.

3. In the second row you will change the fifth value to: 
    00 (left) 
    01 (top)
    02 (right)
    03 (bottom) <- default value

<h4>
  <br>
  <img src="https://raw.githubusercontent.com/marcel-kraatz/windows11-mods/main/StuckRects3.png">
  <br>
  <img src="https://raw.githubusercontent.com/marcel-kraatz/windows11-mods/main/stuckrects.png">
  <br>
</h4>


Then restart explorer.exe or just restart the PC

**OPTIONAL**
If you have multiple displays and multiple taskbars (why?) then you can change it here:

(4). HKEY_CURRENT_USER\SOFTWARE\Microsoft\Windows\CurrentVersion\Explorer\MMStuckRects3
        Repeat the Steps 3 and 4 for each value




# Taskbar_size

1. Navigate to: HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\

2. Do a quick leftklick in the right field select New -> DWORD-Value (32 bit)

3. Name this new value TaskbarSi

4. Then double click the Value and change the value to: 
    0 (small) 
    1 (medium)
    2 (large)

Then restart explorer.exe or just restart the PC

# Classic_Menu.

1. Navigate to: HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Explorer\Advanced

2. Do a quick leftklick in the right field select New -> DWORD-Value (32 bit)

3. Name this value Start_ShowClassicMode and change the value to:
    0 (New Windows 11 Menu)
    1 (Good old Windows 10 Menu) <- I prefer this because i have all my stuff there to keep my desktop clean

Then restart explorer.exe or just restart the PC
