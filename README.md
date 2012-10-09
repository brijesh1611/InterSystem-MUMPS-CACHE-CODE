InterSystem-CACHE MUMPS CODE
============================
Compile the csp file using terminal
Do $system.CSP.LoadPage("/csp/user/mypage.csp","ck")
---------------------------------------------------------------- 
include Caché ObjectScript variables in an alert message
Use #()# syntax. From inside your Caché ObjectScript method, try something like this: 
 s error = "Bad password"
 &js<alert(#(..QuoteJS(error))#);>
The QuoteJS method provided by the %CSP.Page class returns a properly quoted JavaScript string. It also correctly escapes any quotes contained within the returned result.
----------------------------------------------------------------------