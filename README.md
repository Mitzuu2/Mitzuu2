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
