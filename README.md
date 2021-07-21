# clearmap-style
styling for clear map

# Start Docker
```zsh
git clone https://github.com/ubukawa/clearmap-style  
cd clearmap-style  
``` 
Then, edit the hocon files in hocon-xxx to be compiled as style.json.  
Once you are ready, start Docker.  
```zsh
Docker run -it --rm -v ${PWD}:/data unvt/nanban  
cd /data
```  

# Run the hocon-parse
```zsh
rake plain
rake dark
rake gray  
```  
You will get the file in htdocs folder

  