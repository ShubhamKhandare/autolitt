# Autolitt

Autolitt is an application utilising the Tuya API to automatically change SmartLife/Tuya lights as per content on screen.

Tested on following platforms with Wipro WiFi bulb. [Amazon link](https://www.amazon.in/Enabled-12-Watt-Million-Compatible-Assistant/dp/B07S5TH6BN/ref=sxts_sxwds-bia-wc-nc-drs1_0_mod_primary_lightning_deal?crid=2KQBTV463G3E5&cv_ct_cx=wipro+smart+bulb&dchild=1&keywords=wipro+smart+bulb&pd_rd_i=B07S5TH6BN&pd_rd_r=e05125c3-d87f-4bf1-b863-5f10b0fe0f33&pd_rd_w=SwM2D&pd_rd_wg=6uLP4&pf_rd_p=4856a1b6-75e2-4f99-bb59-edf3db6a4f74&pf_rd_r=49R22RCMHSVKVF72ZEJ2&psc=1&qid=1610544877&sbo=Tc8eqSFhUl4VwMzbE4fw%2Fw%3D%3D&smid=AT95IG9ONZD7S&sprefix=wipro+s%2Caps%2C283&sr=1-1-606822b7-04c2-4c74-a611-acbe80e94641)
1. Ubuntu 20.04 LTS
2. Windows 10


### Installation

Autolitt requires [Python 3](https://www.python.org/downloads/) to run.

Install the requirements and run the script.

```sh
$ pip3 install -r requirements.txt
$ python3 autolitt.py
```

You will also need to alter the config.json file with the following:
 1. Your Tuya/SmartLife login and password so it looks like this {"username":"example@domain.com","password":"YOURPASS"...}
 2. Your country code ("91" for India users, 44" for UK users, "1" for US/Canadian users, etc)
 3. The application you're using ('tuya' for tuya users and 'smart_life' for smart life users)

```
{"username":"example@domain.com","password":"YOURPASS","country_code":"91","application":"smart_life"}
```

Inspired from: [Reddit Post](https://www.reddit.com/r/homeautomation/comments/dz677b/heres_how_to_use_wipros_smart_lights_with_ifttt/?utm_source=share&utm_medium=web2x&context=3)

To find the dominant colour I have used https://github.com/fengsp/color-thief-py


### Todos

 - Dynamic Screen Resolution and offset setting
 - Properly adjusting dark and white dominant color

