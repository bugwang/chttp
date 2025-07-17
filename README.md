# cohttp
idea：
http server api ，http client api:
use epoll 
use pool
use coroutine
and Don't depend on third party or only header file
but i need time

desc：

        server
        one loop per pthread  - > co_pool per loop -> ( one request one co)  for  parallel hander

        hander
        a or s io for (one request -> more demand -> parallel demand per co -> one reply)

        
