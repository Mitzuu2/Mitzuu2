0B34: samp register_client_command "comanda1" to_label @cmd_10
0B34: samp register_client_command "comanda2" to_label @cmd_11
0B34: samp register_client_command "comanda3" to_label @cmd_12

0AB1: call_scm_func @chatmsg 0

:cmd_7979
wait 0
jump @cmd_7979

:cmd_10
SAMP.IsCommandTyped(20@)
 chatmsg "Comanda1 [/comanda1]"
SAMP.CmdRet()

:cmd_11
SAMP.IsCommandTyped(20@)
if
0AD4: 20@ = scan_string 20@ format "%d" 21@
then
 0B36: samp 1@ = get_player_nickname 21@
 0AF9: samp say_msg "%s, scrie [/comanda2]" 1@
else
 {FFFFFF}chatmsg "{FFCC66}Syntax: {FFFFFF} Message"
end
SAMP.CmdRet()

:cmd_12
SAMP.IsCommandTyped(20@)
 chatmsg "Comanda3 este [/comanda3]"
SAMP.CmdRet()

:chatmsg
0AA2: 0@ = load_library "samp.dll" // IF and SET
0085: 1@ = 0@ // (int)
1@ += 2203876
0A8D: 3@ = read_memory 1@ size 4 virtual_protec 1
0085: 2@ = 0@ // (int)
2@ += 409616
chatmsg "Message" -1
0AB2: ret 0
0B34: samp register_client_command "comanda1" Unde doresti sa ajungi? @cmd_10
0B34: samp register_client_command "comanda2" Multimim, sa mai folositi serviciile noastre! @cmd_11
0B34: samp register_client_command "comanda3" /ticker (Player 0000_Id @cmd_12
0B34: samp register_client_command "comanda1"  @cmd_10
0B34: samp register_client_command "comanda2" to_label @cmd_11
0B34: samp register_client_command "comanda3" to_label @cmd_12

{$CLEO}
 
0662: ""
thread "" 
wait 2500 
0B34: samp register_client_command "taxihelp" to_label @cmd_1           
{$CLEO}
 
0662: ""
thread "" 
wait 2500 
0B34: samp register_client_command "taxihelp" to_label @cmd_1
0B34: samp register_client_command "tapina" to_label @cmd_2

0AB1: call_scm_func @chatmsg 0                                                                                                                                                                                                                                     
:SYNDER_3
wait 0 
jump @SYNDE
      R_3

:cmd_1
   SAMP.IsCommandTyped(0@)
0AC6: 17@ = label @SYNDER_2 offset 
SAMP.ShowDialog(7777, "", 17@, "", "", cmd 0 SpawnCar441-Gob-1Give-2car 411To
SAMP.CmdRet

:SYNDER_2
hex

end


 :cmd_2
SAMP.IsCommandTyped(20@)
    0AF9: samp say_msg "Salut, unde doresti sa ajungi?"
SAMP.CmdRet()                                              @cmd_1


:chatmsg
@SYNDER_3 0@ = load_library "samp.dll" // IF and SET 
0085: 1@ = 0@ // (int) 
1@ += 2203876 
0A8D: 3@ = read_memory 1@ size 4 virtual_protect 1 
0085: 2@ = 0@ // (int) 
2@ += 409616 
chatmsg "" -1
chatmsg "" -1
0AB2: ret 0
0B34: samp register_cl

0AB1: call_scm_func @chatmsg 0 

:SYNDER_3
wait 0 
jump @SYNDER_3

:cmd_1
   SAMP.IsCommandTyped(0@)
0AC6: 17@ = label @SYNDER_2 offset 
SAMP.ShowDialog(7777, "", 17@, "", "", 0)
SAMP.CmdRet
s
0AB2: ret 0
Chatmsg 1Apasa /Q pentru a face acest lucru!
chatmsg-1Apasa 1Tasta 22 2pentru 1a -2face -8acest -9lucr
@cmd_2 
SAMP:
OAF9: 1samp_say_msg_Salut, 1_unde_doresti_sa_ajungi_?0B34: samp register_client_command "comanda1" to_label @cmd_10
0B34: samp register_client_command "comanda2" to_label @cmd_11
0B34: samp register_client_command "comanda3" to_label @cmd_12

0AB1: call_scm_func @chatmsg 0

:cmd_7979
wait 0
jump @cmd_7979

:cmd_10
SAMP.IsCommandTyped(20@)
 chatmsg "Comanda1 [/comanda1]"
SAMP.CmdRet()

:cmd_11
SAMP.IsCommandTyped(20@)
if
0AD4: 20@ = scan_string 20@ format "%d" 21@
then
 0B36: samp 1@ = get_player_nickname 21@
 0AF9: samp say_msg "%s, scrie [/comanda2]" 1@
else
 {FFFFFF}chatmsg "{FFCC66}Syntax: {FFFFFF} Message"
end
SAMP.CmdRet()

:cmd_12
SAMP.IsCommandTyped(20@)
 chatmsg "Comanda3 este [/comanda3]"
SAMP.CmdRet()

:chatmsg
0AA2: 0@ = load_library "samp.dll" // IF and SET
0085: 1@ = 0@ // (int)
1@ += 2203876
0A8D: 3@ = read_memory 1@ size 4 virtual_protec 1
0085: 2@ = 0@ // (int)
2@ += 409616
chatmsg "Message" -1
0AB2: ret 0
