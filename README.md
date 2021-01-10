# Autolitt

Autolitt is an application utilising the Tuya API to automatically change SmartLife/Tuya lights as per content on screen.
Works on Wipro WiFi bulb

### Installation

Autolitt requires [Python 3](https://www.python.org/downloads/) to run.

Install the requirements and run the script.

```sh
$ pip3 install -r requirements.txt
$ python3 autolitt.py
```

You will also need to alter the config.json file with the following:
 1. Your Tuya/SmartLife login and password so it looks like this {"username":"example@domain.com","password":"YOURPASS"...}
 2. Your country code ("44" for UK users, "1" for US/Canadian users, etc)
 3. The application you're using ('tuya' for tuya users and 'smart_life' for smart life users)

```
{"username":"example@domain.com","password":"YOURPASS","country_code":"44","application":"tuya"}
```


### Todos

 - Dynamic Screen Resolution and offset setting
 - Properly adjusting dark and white dominant color

