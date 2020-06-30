# dsalg














# Poetry Setup

1. poetry new datagen OR
   if the folder already exist poetry init
2. cd datagen
3. poetry install  ( Creating virtual environment, It will also give the path where Virtual environment has been created )
4. Open the project in VS Code
5. Configure the setting to add virtual environment in VS Code workspace with below settings:
{
    //Basic Setup Configurations
    "terminal.integrated.shellArgs.windows": [
        "-ExecutionPolicy",
        "Bypass"
    ],
    "files.associations": {
        "*.toml": "ini",
    },
    //Editor Configurations
    "editor.minimap.enabled": false,
    "editor.fontSize": 18,
    "editor.formatOnSave": true,
    //Python configurations
    "python.venvPath": "C:\\Users\\sk\\AppData\\Local\\pypoetry\\Cache\\virtualenvs",
    //"python.pythonPath": "C:\\Users\\sk\\AppData\\Local\\pypoetry\\Cache\\virtualenvs\\how-long-46llcXc5-py3.6\\Scripts\\python.exe",
    "python.formatting.provider": "black",
    "python.formatting.blackArgs": [
        "--line-length",
        "88"
    ],
    "python.linting.enabled": true,
    "python.linting.pylintEnabled": true,
    "python.linting.pylintArgs": [
        "--max-line-length=88"
    ]
}

6. After this refresh the window and choose the python path of your respect virtualenv path. It will add python.pythonPath entry in settings.xml
7. Ater this add pylint and black
8. Adding Dependencies 
	poetry add [package-name]
	
9. Adding Dev Dependencies
		poetry add -D [package-name]

10. Removing dependencies
        poetry remove [package-name]        
