# ModEngine2 - Способ обхода
Не имея лицензионной копии Elden Ring`a , становится проблематично поиграть со всеми модами, которым нужен **ModEngine2**

## Первый способ - Metis_Launcher
![image](https://github.com/user-attachments/assets/d6ea49d0-dcfb-41da-a305-bc6e3761fc4e)
https://github.com/HazelnutCheese/Metis-Mod-Launcher

На удивление при попытках запустить тот же **Reforged** или **The Convergence** через установленный отдельно **ModEngine2** , я сталкнулся с рядом проблем, но в лаунчере всё было иначе.
### Единственно над чем стоит заострить внимание :
> Правильность указания папки мода
>> Порядок загрузки
>>> Чистая версия игры ( В нашем случае Crack`ed )

## Второй способ - ModEngine2

На просторах интернета нашёл несколько способов, по заветам которого ваш ModEngine2 должен после этого заработать :
![image](https://github.com/user-attachments/assets/6c67365a-9cb1-4cf4-94c9-a1a73bb9d39d)
![image](https://github.com/user-attachments/assets/bd8c1d94-e925-4f72-850d-8b73559a1e04)
![image](https://github.com/user-attachments/assets/11a7c553-e283-43f7-80fa-9d015b82d79a)
### ССылки из ресурса :
> You can also follow this tutorial: https://winaero.com/add-open-in-windows-terminal-as-administrator-to-context-menu/
>> If you are still having problems, check this reply post of someone who seems to have been able to make it work just by throwing ModEngine2 in the same folder. https://www.reddit.com/r/PiratedGames/comments/u55adf/comment/ig7uz2t/?utm_source=reddit&utm_medium=web2x&context=3
>>> Ссылка на Reddit-Пост https://www.reddit.com/r/PiratedGames/comments/u55adf/elden_ring_modding_with_mod_engine_2/

### Альтернативный способ 

Ok, let me see if I can give you what you need.
Soup-to-Nuts:
Download DSL and ModEngine2:

Go here: https://www.nexusmods.com/eldenring/mods/2777?tab=description
Navigate a little down the page and you will see "Installation" this has a link to ModEngine2.
You can follow these instructions which will keep your normal elden ring directory untouched.
Once ModEngine2 is downloaded, you will need to 'right-click' and extract it to your desired location.
-- I installed mine on my desktop for quick access.
Navigate into your ModEngine2 folder which if left default should be 'ModEngine-2.0.0-preview4-win64'
-- In this folder you will see a 'mod' folder.
Download 'DSL' from the link in step 1
Extract the DSL mod into the mod directory. so the folder directory would look something like:
This PC > Desktop > ModEngine-2.0.0-preview4-win64 > mod >DSL Beta 0.5 (Reupload)-2777-Beta05-1675030644
Navigate to This PC > Desktop > ModEngine-2.0.0-preview4-win64 > mod
Optional (What I did): Right click the folder DSL Beta 0.5 (Reupload)-2777-Beta05-1675030644 and select Rename. Change this to just 'DSL-Beta'
You will see many files but the ones that we care about are:
a) config_eldenring.toml
b) launchmod_eldenring.bat
First Right-click the config_eldenring.toml then select  Open with... A new window will open allowing you to select an app. We are looking for notepad.
---- Note, you might have to select 'more options' in the new window for the app to show up. -----
you want to make sure you have the following line:
mods = [     { enabled = true, name = "default", path = "mod\\DSL-Beta" } ]
Click on 'File' at the top of the notepad app and then click save
Once that line exists the assumption is your mod is installed at This PC > Desktop > ModEngine-2.0.0-preview4-win64 > mod > DSL-Beta
Now close the notepad window for the 'config_eldenring.toml'
Right-click the launchmod_eldenring.bat and select Edit1 which should open notepad`
----- This is different because the file extension is .bat which is a script that can be run -------
Now with this open you will probably only see:
.\modengine2_launcher.exe -t er -c .\config_eldenring.toml
add the following:
.\modengine2_launcher.exe -t er -c .\config_eldenring.toml --game-path "D:\SteamLibrary\steamapps\common\ELDEN RING\Game\eldenring.exe
Finally click File at the top of the notepad and click Save
Double-click the launchmod_eldenring.bat and you should be off to the races.
-------------- Ensure that you change the path in between the " " to that of your path to your eldenring.exe --------------

A quick way to find this path is to go to ELDEN RING in Steam Right-Click and hover over manage and select Browse Local Files

which will open an explorer window and you should have a folder called Game

navigate into the Game folder click on the navigation bar in the white space and it will change from This PC > Path > To > SteamLibrary >  steamapps > common > ELDEN RING > Game to something like D:\SteamLibrary\steamapps\common\ELDEN RING\Game




