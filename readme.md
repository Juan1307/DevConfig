# Dev config

Anotaciones y configuración para: **win-terminal**, **cursor-editor** y **.git**

- Windows Terminal.
- Cursor Editor.
- Git.

## ```/terminal```

Configuración inicial para la terminal de windows con persistencia a comandos y atajos:

**- Paso 1**: Crear una carpeta para _**macros**_ con el archivo ejem: ```C:/bat/macros.doskey```.

**- Paso 2**: Ir al registro de windows ```Win + R```  ingresa el comando _**regedit**_ y la ruta ``` HKEY_LOCAL_MACHINE\Software\Microsoft\Command Processor\ ``` y crear el archivo ```Autorun``` como ```String Value``` y en su value setear ```DOSKEY /MACROFILE="C:\bat\macros.doskey"``` al macrofile con el path de nuestro macros.

**- Paso 3**: Al abrir **Windows terminal** ir a la configuración y en **Prompt command**  verificar que el _profile_ de la linea de comandos apunte a ```C:\WINDOWS\System32\cmd.exe``` por defecto hace referencia al ```%SystemRoot%```

**- Paso 4**: El archivo adjunto en ```/terminal``` contiene comentarios basados en la sintaxis ```.bat``` eliminarlos para omitir el error ```invalid macro definition.```

**Recursos y referencias**:

- DOSKEY persistent: https://superuser.com/questions/1134368/create-permanent-doskey-in-windows-cmd
- MSDOS commands: https://learn.microsoft.com/en-us/windows-server/administration/windows-commands/doskey
- PROMP syntaxt: https://ss64.com/nt/prompt.html

## ```/editor```

Configuración para **cursor-editor** y cambiar los _**shortcuts**_, _**themes**_ y  _**extensions**_:

**- SHORTCUTS**: Para configurar los shortcut parecidos a los de sublime instalar la extension ```Sublime Text Keymap and Settings Importer``` e ir a **Preferences>Open Keyboard shortcuts JSON** y copiar el json de ```/editor/keybindings.json```.

**- THEMES**: Para configurar parte del tema agregar el tema **EgoistOne** e ir a **Preference>Open User Settings Json** y copiar el json de ```/editor/settings.json```.

**- EXTENSIONS**: --- sin config ---

## ```/git```

Configuracion para .git:

- Usar el archivo config de ```/git``` y el archivo ```config``` para administrar **.ssh** en la ruta ```C:\Users\antik\.ssh```.
- Usat el archivo ```.gitconfig``` para setear los atajos en **git** en la ruta base de ```C:\Users\antik```.
