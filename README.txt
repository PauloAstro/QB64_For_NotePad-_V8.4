*****************************************************************
*																                                *
*         QB64 language files for NotePad++ v.8.4.4 64bits		  *
*																                                *
*																                                *
*****************************************************************


First Edition by PauloAstro at 14 August 2022. 
Last reviewed at 18 Aug 2022.


0) Introduction.
1) Language files installation.
2) Config NotePad to use F5 key to compile .bas files.
3) Revision Version History.
		
0) Introduction --------------------------------------------------------


This QB64 language implementation on NotePad++ (v.8.4.4, 64bits) Portable edition uses only 3 configuration files (.xml) to be copied to the NP++ folders:
	1 - qb64_UDL_vX.XXX.xml/qb64_UDL_DarkMode_v0.XXX.xml - file that holds the language keywords and rules based on the User Design Language interface for NP++. The "DarkMode" file should be used when using the DarkMode on NP++. The colors are similar to the QB64 Original IDE.
	2 - QB64FL.xml - file that holds the rules that to identify the Functions and Subroutines used on .bas .bi and .bm files for the QB64 language.
	3 - overrideMap.xml - Add only one configuration line (<association id="QB64FList.xml" userDefinedLangName="QB64"/>) that tels NP++ the FunctionList rules to be used for QB64 user defined Language (UDL).
	    

1) Language files installation -----------------------------------------

	1.1) Copy qb64_UDL_v0.XXX.xml to the userDefineLangs folder.
	1.2) Copy QB64FList.xml to the functionList folder of NP++.
	1.3) Copy overrideMap.xml to the functionList folder or just edit overrideMap.xml adding the following code line:
		<association id="QB64FList.xml" userDefinedLangName="QB64"/>
	     as explained inside the overrideMap.xml to the existing file if you have more than one UDL FunctionList rules.


2) Config NotePad++ to use F5 key to compile .bas files  -------------------

	2.1) Copy QB64_noIDE.exe to your QB64 folder, aside with QB64.exe.
	2.2) Configure manualy windows 10 to open all .bas files with QB64_noIDE.exe, selecting the "Open With.." option for any .bas file.
	2.3) Install the "RunMe" plugin on NP++, and restart it.
	2.4) On NP++ Settings -> Shortcut Mapper -> Main menu, and look on 'Filter' for the 'Run' NAME and change the shortcut key from F5 to F6 (for exemple). And click 'Modify'.
	2.5) At the 'Plugin commands' look for 'Shell execute current file' and edit the Shortcut to F5.

	Now when pressing F5 it will compile the active NP++ document with QB64_noIDE.exe.



3) Revision Version History  -----------------------------------

	Rev.01 - 17 Aug 2022.
		- Updated QB64FList.xml
		- Updated UDL to qb64_UDL_v0.003.xml
		- Added new qb64_UDL_DarkMode_v0.003.xml for DarkMode color Preferences.

	Rev.00 - 15 Aug 2022.
	

