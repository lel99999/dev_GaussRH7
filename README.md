# dev_GaussRH7
Gauss update for RHEL 7.x from v15 to v20

#### Add for XWindows 
Use:
$yum groupinstall "Server with GUI"<br/>

Instead of:
$yum groupinstall "X Window System"<br/>

#### Add Library Path
Testing for verification:<br/>
1:<br/>
`lib <path_to_lib> -addpath`<br/>

2:<br/>
Under library tool -> Under Paths -> Right-Mouse-Button -> Add Files <br/>

##### Library Source & Example
1) Download carrionlib.zip from https://github.com/aptech/gauss-carrion-library/releases
2) Select Tools -> Install Applications from main Gauss Menu
  2a) Make sure /usr/local/gauss20/pkgs is created and writable
3) Follow installer prompt
4) Before using functions created by carrionlib, need to load the newly created carrionlib library:
  4a) Navigate to Library Tool Windows and click on small wrench located next to the carrionlib library. Select load library
  4b) Enter library carrionlib in Porgram Input/Output Window
  4c) Put the line library carrionlib; at the beginning of your program files

##### Add Library Path to /home/<org>/<username>/gauss20/gauss.cfg
`extra_lib_path = /<path_lo_libraries>/`<br/>

Right-mouse-button click on Library Tool to load library<br/>
