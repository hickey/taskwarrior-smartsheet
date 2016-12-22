# taskwarrior-smartsheet

Taskwarrior extension for using a Smartsheet project or task list sheet for organizing a project. 

## Installation

In order for this Taskwarrior extension to be used, one must install the following Python modules. This can be done by executing `pip install <module>`
    
    * taskw
    * smartsheet-python-sdk




## Usage

    usage: task-ss [-h] [--list [SEARCH_TEXT [SEARCH_TEXT ...]]] [--sheet ID]
                   [--key API_KEY] [--project NAME] [--default-key API_KEY]
                   [--config FILE]
    
    Taskwarrior to Smartsheet Sync
    
    optional arguments:
      -h, --help            show this help message and exit
      --list [SEARCH_TEXT [SEARCH_TEXT ...]], -l [SEARCH_TEXT [SEARCH_TEXT ...]]
                            List available Smartsheets
      --sheet ID, -s ID     Smartsheet ID to setup a sync for
      --key API_KEY, -k API_KEY
                            Specify API key to access sheets
      --project NAME, -P NAME
                            Taskwarrior project to associate with sheet
      --default-key API_KEY, -K API_KEY
                            Set default Smartsheet API key
      --config FILE, -f FILE
                            Read specified config file for API keys


### Searching for sheets

    task-ss --list foo
    task-ss --list foo '!bar'
    