# Unity Script Templates

This repository is a bundle of the Script Templates I use in my Unity Projets.

## Setup Script templates in Unity

What I'm calling Script Templates are the scripts generated by Unity when you create a new C# Script for examples.

They are written in your Unity Installation, in `Editor/Data/Resources/ScriptTemplates`. You can notice a specific file naming, see below for more informations about that.

To setup my custom Unity script tempates, download or clone this repo into your Unity install folder. If your Unity editor is open when you set these files, close it and reopen it.

```bash
git clone https://github.com/thatgamecoder/unity-script-templates.git
```

Now, if you try to create a new Asset (by right-clicking in the `Project` view, or from `Assets` menu), you can see some new menus for script creation !

![Create asset menu example](menu-example.png)

Obviously, you can create your own script templates, or simply adapt mines for your common usage.

## Script Templates naming

You can see that all the template scripts files have a specific naming syntax :

```
85-Other Scripts__Scriptable Object-MyClass.cs.txt
```

Let's see the composition of that... thing :

| 85 | Other Scripts | Scriptable Object | MyClass | .cs |
| - | - | - | - | - |
| Menu position | Menu name | Submenu name | Default name of the new created file | Created file extension |

Note that submenus are facultative, but you can setup as many submenus as you want, by separating elements with "`__`".

## Script Template content

You can make script templates of any text asset you want (it can be C#, JSON, XML, YAML, TXT, or any code or text content).

Inside these scripts, you can also use `#SCRIPTNAME#` keyword. When Unity generates the new asset, it will replace that keyword by the created file name. It can be useful for automating class name generation.
