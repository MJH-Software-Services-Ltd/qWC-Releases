# qWC
Emulation and extension to ⎕WC from Dyalog APL

Take the Examples.pdf as they give examples of most of the controls

To install take the Zip and extract Output dir

If on Windows and it goes to c:/Dyalog/cmd/QWC/Output then no config changes are needed
Copy the two files QWC.dyalog and QWC.dcfg from Output to your User Command folder - see Dyalog's User Command manual for details

If the directory is different then the config QWC.dcfg will need to be edited - both outputdir and defaultbrowser to suit (Local, Chrome, Edge, Firefox to choice) - Local is HTMLLRenderer

On a Mac dpownload the same files

Place the Output in a directory say as /Users/id/Output
Put the QWC.dyalog and QWC.dcfg into /User/id/MyUCMDs and edit QWC.dcfg with the path and set the browser to Safari or Local (HTMLRenderer)

On some releases of Dyalog 18 18.2 and 19 there is a bug preventing Safari or HTMLRenderer from starting automatically. If you have a later 19 or earlier 18 or 18.2 then it will work, others will need the additional step of starting Safari manually to complete the inmitialization.

If ]qwcinit starts and produces "* qWC initialized" then this is good and this is the client screen.

If it doesnt start properly then as a temp soln you need to enter qSafari '' in the other window after
* Client Server started on port 1236   (this is the framework window which is normally minimized or set as an APL service) 

  Type qSafari ''
  You should then get *** User Id set to 1

  In the other Window after * Attempting to connect to the Client Web Socket
  you shoukd get

  * qWC Initialized
 
    If so you are good to use the window after * qWC Initialized as before

   Please note : Most if not all the examples use #.qWC/G/S but these actions can be done using#.qNew and ns.ns1.prop←action   as in fn.btn1.BCol←'red'
  instead of 'fn.btn1' #.qWS 'BCol' 'red'
  
  :with 'f' #.qWC 'Form'
       'b1' #.qWC 'Button' ('Style' 'Push')
       'b2' #.qWC 'Button' 'Push' 
  :endwith
    is also supported 


MORE INFO will be added asap but we will help you with the installation.
