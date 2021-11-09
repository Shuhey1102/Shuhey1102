- 👋 Hi, I’m Shuhey
- 👀 I’m interested in creating amzing and exciting program by myself
- 🌱 I’m currently learning Java,JavaScript,HTML,CSS,Python,Uipath,OutSystems
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ... shuheylab@gmail.com

<!---
Shuhey1102/Shuhey1102 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.0-beta1/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-giJF6kkoqNQ00vy+HMDP7azOuL0xtbfIcaT9wjKHr8RbDVddVHyTfAAsrekwKmP1" crossorigin="anonymous">
    <style>
        .canvas{
            background-color:limegreen;
            border:black solid 2px;
            
        }
        dt{
            border:1px solid;
            padding: 5px;
            width: 462px;
        }
        dt:before{
            content:">";
            font-size:.8em;
            padding-right:5px;
        }
        dd ul{
            list-style: none;
            padding: .5em;
        }
        .PlayerScreen{
            display: none;
            margin: none;
        }
        .Player1{
            padding-right: 10px;
            padding-left: 7px;
            padding-top: 15px;
            padding-bottom: 20px;
            background-color:#ffff;
            border:1px solid;
            border-radius: 10px
 
        }
        .Player2{
            padding-right: 10px;
            padding-left: 7px;
            padding-top: 15px;
            padding-bottom: 20px;
            background-color:#ffff;
            border:1px solid;  
            border-radius: 10px;
            margin-left:10px
        }
        .messageStyle{
            font-size: 20px; 
            margin-top: 10px;
            margin-bottom: 10px;
        }
    </style>
    <title>Osero</title>
    </head>
    <body style = "margin-left:70px;background-color:gainsboro; width:800px;height:1000px;">
    <div>
        <div style="font-size: 50px; margin-bottom: 10px;">Osero
        </div>  
        <div>
            <dl class="option">
                <dt>Options</dt>
                <dd>
                    <ul>
                        Player1:
                        <select id="Player1" style="margin-top:15px;">
                            <option>
                                Player
                            </option>
                            <option>
                                CPU
                            </option>
                        </select>
                    </ul>
                    <ul>
                        Player2:
                        <select id="Player2" >
                            <option>
                                Player
                            </option>
                            <option>
                                CPU
                            </option>
                        </select>
                    </ul>
                </dd>
            </dl>   
        </div>
        <div style="margin-bottom: 10px;">
            <button id ="StartButton" type="button" class="btn btn-primary btn-lg" onclick=StartOsero()>Start</button>
            <button type="button" class="btn btn-secondary btn-lg" onclick=ResetOsero()>Reset</button>
        </div>
        <div id="messageStyle">
            <div class = "messageStyle">
                Message&nbsp;:&nbsp;
                <span id = "message"></span>
            </div>    
        </div>
        <div id = "PlayerScreen"class="PlayerScreen">
            <h3>
              <span class="Player1">Player1&nbsp;&nbsp;<img id="Player1img" src="../Osero/image/boy_init.png" width="40px" height="60px">&nbsp;<img src="../Osero/image/osero_black.png" width="50px" height="30px"></span>
              <span class="Player2">Player2&nbsp;&nbsp;<img id="Player2img" src="../Osero/image/girl_init.png" width="40px" height="60px">&nbsp;<img src="../Osero/image/Osero_white.jpg" width="50px" height="30px"></span>
             </h3>               
         </div>  
    
        <div style="margin-top: 10px;">
            <canvas id ="can1" width="50" height = "50" class = canvas onclick = PutOsero()>
            </canvas>
            <canvas id ="can2" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can3" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can4" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can5" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can6" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can7" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can8" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>       
            <br>
            <canvas id ="can9" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can10" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can11" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can12" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can13" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can14" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can15" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can16" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <br>
            <canvas id ="can17" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can18" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can19" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can20" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can21" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can22" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can23" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can24" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas><br>
            <canvas id ="can25" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can26" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can27" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can28" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can29" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can30" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can31" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can32" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <br>
            <canvas id ="can33" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can34" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can35" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can36" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can37" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can38" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can39" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can40" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas><br>
            <canvas id ="can41" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can42" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can43" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can44" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can45" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can46" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can47" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can48" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas><br>
            <canvas id ="can49" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can50" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can51" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can52" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can53" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can54" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can55" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can56" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas><br>
            <canvas id ="can57" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can58" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can59" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can60" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can61" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can62" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can63" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <canvas id ="can64" width="50" height = "50" class = canvas onclick = PutOsero() >
            </canvas>
            <br>
        </div>
    </div>
    <script src="./jquery-3.6.0.min.js"></script>
    <script src="./osero.js" ></script>   
</body>
</html>
