Lay-outs in Github: https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

*Login to remote machine:* ``` ssh ubuntu@149.165.157.40```   
*See the history of the commands:* ```$ history```  
*Help for a command:* ```$ command --help ```  
*Find path of working directory:* ```$ pwd ```  
*Data folder (as ubuntu user):* ```/home/ubuntu/data/drone``` 
*Remove files:* ```$  rm -i file```  
*Nano go to end of line:* ```$  ctrl+w+v```

*Go back to the normal ubuntu user*: ```$ exit```    
*What user am I:* ```$ whoami ``` 
*Edit documents with:* ```$ nano -w filename``` 
Edit this new resource configuration file:  
```$ nano -w /etc/vts/mapproxy/sandwich.d/sandwich_ortho.json```  

*ctrl+x to exit: it will ask to save, (say yes) and then the file name, type it and enter*  

*Change working directory:* ```$ cd data/drone ```  
*List everything in directory:* ```$ ls data/drone ```  
*Check if directory exists:* ``` $ [ -d /home/ubuntu ] && echo 'Directory found' || echo 'Directory not found'```  
*Check if file exists:*``` $ [ -f /home/ubuntu ] && echo 'File found' || echo 'File not found'```
*Make directory:* ```$ mkdir /var/vts/mapproxy/datasets/sandwich```  
*Copy files (works only if you're logged in as the vts user):*  
```$ cp /home/ubuntu/data/drone/2017-03-16_Sandwich_v1_ORTHO_10cm.tif /var/vts/mapproxy/datasets/sandwich```  

*Bash paths on local computer:*  
*Normal paths:*```"C:\Users\Gebruiker\Downloads\Targets_planned_for_10-Jan-2018.kmz"```  
*Ubuntu paths:*```"/mnt/c/Users/Gebruiker/Downloads/Targets_planned_for_10-Jan-2018.kmz"```  

*Copy file from local computer to a remote machine (as local user):*  ```$ scp /mnt/c/Users/Gebruiker/Downloads/Targets_planned_for_10-Jan-2018.kmz ubuntu@149.165.157.40:/home/ubuntu/data/drone```  

*List files from a remote machine:*  ```$ ssh ubuntu@149.165.157.40 ls -l /home/ubuntu/data/drone```  

*Reading .kmz files with gdal package:* ```$ ogrinfo Targets_planned_for_10-Jan-2018.kmz -al -so```  
*Convert .kmz to Geojson:* ```$ ogr2ogr -f GeoJSON Targets.json Targets_planned_for_10-Jan-2018.kmz```  