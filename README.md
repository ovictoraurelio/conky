## Conky configuration
<img src='1920x1080.jpg' width='900px'>

## Installation
- Clone repo `git clone https://github.com/alexbel/conky.git ~/.conky`
- Install dependencies (see below)
- Install the necessary ruby gems (see below)
- Rename secrets.yml.example to secrets.yml and put your data in it
- Run 'ruby starter.rb' or just './starter.rb'

## Autostart
Kde plasma 5:  
Create a file `conky.desktop` in `~/.config/autostart` directory and fill it in with the following contents:  
```
[Desktop Entry]
Name=conky
Exec=cd ~/.conky && ruby starter.rb
Type=Application
Terminal=false
```

### Conky versions
- Use `master` branch for conky >= 1.10.0
- Use `1.9` branch for conky <= 1.9.1

### Dependencies
Required:  
  - curl
  - ss
  - acpi
  - sensors
  - Install Conky 
  
```
$ sudo apt-get install conky conky-all
```

Conky libs:  
  - conky-imlib2
```
$ sudo apt-get install build-essential automake git docbook2x libxfixes-dev libasound2-dev libcairo2-dev libcurl4-gnutls-dev libglib2.0-dev libimlib2-dev libiw-dev liblua5.1-0-dev libncurses5-dev libtolua++5.1-dev libtool libx11-dev libxdamage-dev libxext-dev libxft-dev libxml2-dev 
```
Gmail:  
  - ruby >= 1.9.3

  gems:  
  - ruby-gmail
  - mime
```
$ gem install ruby-gmail
$ gem install ruby-gmail
```

Weather:  
  - [wunderground](https://github.com/wnadeau/wunderground) gem
  - api_key from http://www.wunderground.com/weather/api/
