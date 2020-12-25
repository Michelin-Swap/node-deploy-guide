linux运行环境，ubuntu 20.04  
1. 复制文件：   
cp libgo_cosmwasm.so /usr/lib  
cp wasmd wasmcli /usr/bin  

2. 初始化  
wasmd init --chain-id=MidasEcological  

3. 复制 genesis.json 到 ~/.wasmd/config/ 文件夹。  
4. 添加seed，方法：编辑 ~/.wasmd/config/config.toml 的 seeds。  
   文件seeds.txt里的内容就是seeds     
  
5. 运行  
   wasmd start  
   
6. rest-server 启动：  
wasmcli rest-server --chain-id MidasEcological --laddr tcp://0.0.0.0:1317 --unsafe-cors --trust-node  


