Interpreter-ScriptCompiler
==========================

Simple script compiler and interpreter


CScriptCompiler:

The class implements a simple compiler for a script language.
It reads a syntax file containing a description of the language
in simplified Backus-Naur Form and builds a syntax graph from there.
It also generates integer codes for all keywords of the language,
as well as the obligoratory code for the "identifier" keyword.
The method compile() checks a script file for syntax errors
and translates the keywords and identifiers in integer codes for
for faster execution. If no errors occured during compilation,
the program, keyword table, and identifier table can be queried.



CInterpreter:

The class implements a simple interpreger for the programs
compiled with CScriptCompiler. It can be used to create simple
graphic or text adventures, among other things. Define
objects that represent different scenes in the adventure,
variables that can be used to supply the user with information,
or to represent items or game states. Define procedures that
represent the choices at each stage of the game.



interpreter_test.cpp is a simple example showcasing how the
classes work.
