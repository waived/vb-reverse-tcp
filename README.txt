|==================================|
|====  VB SHELL - REVERSE TCP  ====|
|==================================|

Released on:
      10.29.2024 @ 14:56

Description:
      Via a Reverse-TCP-connection, the 'server.exe' controller can manage
      multiple incoming-connections from devices infected with 'client.exe'

How to use:
      Simply edit the Client project and replace the RHOST and RPORT value
      with the correct IP Address and server Port assigned to the attacker C2.

Note: There are no features/functions built into this shell. It only
      functions as a remote cmd shell into a system. If said command 
      statements sent to the user yield a verbose output, the client.exe
      backdoor will report the output back to the attacker.

      This shell CANNOT manage sessions with devices in a concurrent
      manner, nor switch between sessions. As each device phones-home
      to server.exe you will have the ability to reject or accept each
      incoming connection. After a session is over, enter "goodbye"

      Warning: after "goodbye" is sent, the shell will no longer report
      home. This can be easily modified to revive the connection regardless
      of commands given by the C2. This overall basic shell design servers
      as a basic penetration testing / red teaming program.

Good luck, and use responsibly!
