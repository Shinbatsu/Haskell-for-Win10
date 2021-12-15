# <center>Guide for Instalation Hasekell for Windows 10 x64</center>

## Some Story :hourglass:

During breaks from work, I liked programming in Haskell, but today I wanted to write a Haskell program for windows, this is a little guide at that way if i forget how I did it.

---

## IMPORTANT LINK :wheelchair:

<https://docs.haskellstack.org/en/stable/README/>

## Tutorial :books:

### 1.Installing 'stack' for win10 :arrows_counterclockwise:

1.1 Direct link to the installer :link: : <https://get.haskellstack.org/stable/windows-x86_64-installer.exe>

1.2 Note: Add checker in 'Add to uset %PATH%' :heavy_exclamation_mark:

1.3 If you forgot then <https://docs.microsoft.com/en-us/previous-versions/office/developer/sharepoint-2010/ee537574(v=office.14)>
![Installer](/assets/installer.png)

### 2.Stack Conf :clipboard:

2.1 After installation check path 'C:\\' or 'C:\Users\\(UserName)'

2.2 There should be directory 'sr',go inside and found there 'config.yaml'

2.3 Change this:

```yaml
templates:
  params:
#    author-name:<Name> 1
#    author-email:<Mail> 2
#    copyright:<someField> 3
#    github-username:<Github> 4
```

### 3. First Program :page_with_curl:

3.1 Create somewhere folder and open Windows console from them

3.2 Create project:

```bash
stack new project1
```

![Shell1](/assets/shell1.jpg)

3.3 change directory

```bash
cd project1 OR ABSOLUTE PATH d:/.../.../project1
```

3.4 Use 'stack setup' for installation of compiler to project1

```bash
stack setup
```

3.5 After that you can see file 'Main.hs' inside 'project1/app', this is haskell program

3.6 Used stack build you compile .hs files from 'app' directory to .exe which will be inside ' .stack-work/dist/721ab02d/build/project1 '

3.7 If you want to run your program then write in console

Note: -exe always will be at the end filename

```bash
stack exec project1-exe
```

![Shell1](/assets/shell2.jpg)

### 4. Integration with VS Code \<TODO\> :vs:
