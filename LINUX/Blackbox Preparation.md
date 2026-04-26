

### /dev/null     ----- black hole
```
- speacial file in linux that acts as data black hole . 
- anything weitten to it is discarded forever and reading from it return nothing .
- It is commonly used to suppress command output or errors in shell scripts.
- it exist because we need to throw away ouput constantly . 
  
----- Advantages ----------
-- suppress unwated output
-- baground processes  


```

### /dev/zero    ---- endless zero
```
- When you read from `/dev/zero`, Linux gives you an infinite stream of zero byte
  
- creates empty files of fixed size 
    
- Why is it useful?
		Because sometimes in Linux/admin work you need:
		
		- blank file of fixed size
		- initialize a disk image
		- create swap file
		- overwrite data with zeros
		- benchmark writes
```


### /dev/random
```
- 
```

### /dev/tty
```
-
```

### file types --- special
```
command to see -------    ls -l

---- Linux supports file types like regular files , directories , symbolic links , character devices , block devices , fifo(named pipes) and sockets. 


=>  ( - ) -> regular file ->  text , scripts , configs , binaries
=>  ( d ) -> directories 
=>  ( l ) ->  Symbolic link  -> shortcut /pointer to another file 
=>  ( c ) ->  Character device  -> stream oriented device 
				-> ex - /dev/null  , /dev/zero  , /dev/tty  , /dev/random

=>  ( b )  -> Block device  -> block storage device  -> ex. /dev/sda  , /dev/nvme0n1  , /dev/loop0

=>  ( p )  -> named pipe  / FIFO  -> used for inter-process communication   -> mkfifo mypipe
				-> one way communication --> local communication
				-> fifo behaviour 
				-> simple inter process communication 

=>  ( s )  -> socket  -> interprocess communication  -> docker socket , systemd sockets , database sokets
				-> bi-directional communication 
				-> more flexible 
				-> supports streams or datagram communication 
				-> ex -  Docker client communicates with dockerd  using  /var/run/docker.sock  socket file 







```

