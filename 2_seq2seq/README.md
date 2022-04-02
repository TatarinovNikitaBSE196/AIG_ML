Experiments with [algorithm](https://github.com/xinyadu/nqg) from [this article](http://dx.doi.org/10.18653/v1/P17-1123).  
Failed to make experiments. To run the model, tds package is required:  
```/home/nickyoleary/torch/install/bin/luajit: ...e/nickyoleary/torch/install/share/lua/5.1/trepl/init.lua:389: ...e/nickyoleary/torch/install/share/lua/5.1/trepl/init.lua:389: ...e/nickyoleary/torch/install/share/lua/5.1/trepl/init.lua:389: ...e/nickyoleary/torch/install/share/lua/5.1/trepl/init.lua:389: module 'tds' not found:No LuaRocks module found for tds
	no field package.preload['tds']
	no file '/home/nickyoleary/.luarocks/share/lua/5.1/tds.lua'
	no file '/home/nickyoleary/.luarocks/share/lua/5.1/tds/init.lua'
	no file '/home/nickyoleary/torch/install/share/lua/5.1/tds.lua'
	no file '/home/nickyoleary/torch/install/share/lua/5.1/tds/init.lua'
	no file './tds.lua'
	no file '/home/nickyoleary/torch/install/share/luajit-2.1.0-beta1/tds.lua'
	no file '/usr/local/share/lua/5.1/tds.lua'
	no file '/usr/local/share/lua/5.1/tds/init.lua'
	no file '/home/nickyoleary/.luarocks/lib/lua/5.1/tds.so'
	no file '/home/nickyoleary/torch/install/lib/lua/5.1/tds.so'
	no file '/home/nickyoleary/torch/install/lib/tds.so'
	no file './tds.so'
	no file '/usr/local/lib/lua/5.1/tds.so'
	no file '/usr/local/lib/lua/5.1/loadall.so'
stack traceback:
	[C]: in function 'error'
	...e/nickyoleary/torch/install/share/lua/5.1/trepl/init.lua:389: in function 'require'
	preprocess.lua:1: in main chunk
	[C]: in function 'dofile'
	...eary/torch/install/lib/luarocks/rocks/trepl/scm-1/bin/th:150: in main chunk
	[C]: at 0x563089f6c000
```
However, there are problems with downloading the package due to [GitHub restrictions](https://github.blog/2021-09-01-improving-git-protocol-security-github/):  
```
Installing https://raw.githubusercontent.com/torch/rocks/master/tds-scm-1.rockspec...
Using https://raw.githubusercontent.com/torch/rocks/master/tds-scm-1.rockspec... switching to 'build' mode
Cloning into 'tds'...
fatal: remote error: 
  The unauthenticated git protocol on port 9418 is no longer supported.
Please see https://github.blog/2021-09-01-improving-git-protocol-security-github/ for more information.

Error: Failed cloning git repository.
```