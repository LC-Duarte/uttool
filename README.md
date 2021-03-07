# UTTOOL

Youtube dowload tool

## About

Script for downloading youtube videos

## Options

* -c | --config     Set configuration file path 
* -d | --debug      Activate debug mode
* -o | --output     Set output path
* -s | --source     Set video source URL

## Usage

### Single video download

Use the output and the source options like the example bellow

```bash

$python uttool.py -o <path-to-ouput-folder> -s <url-to-video>

```

### Multiple video dowloads

Edit *".../uttool/cofig_uttool"* and call the scripts with no options or create a new
yaml config file containg *"out_path"* and *"video_list"* like the example bellow:

__NOTE:__ If repetitive links are provided, the script will ignore the second occourence

```yaml

#config_uttool.yaml

out_path: /Users/Leonardo/Google Drive/investimento/curso_mira/video_aulas
video_list:
    - https://www.youtube.com/watch?v=hKY0Z8J1cCU
    - https://www.youtube.com/watch?v=RZuEG-TtmGA
    - https://www.youtube.com/watch?v=DggquAatQNA
    - https://www.youtube.com/watch?v=HFXMxZLW4qA

```

If you edited the default config file (*".../uttool/cofig_uttool.yaml"*) just call the script with no extra options

```bash

$python uttool.py

```

If you opted for a new config file call the script providing the path to that config file

```bash

$python uttool.py -c <config-file-path>

```

## Author
Leonardo Chaves Duarte 

leonardochavesduarte@gmail.com

github.com/LC-Duarte/

Curitiba - Parana - Brazil

