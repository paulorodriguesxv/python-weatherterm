
# Weather Application

Weather request 

Scrape weather forecast information from https://weather.com and present it in a terminal. 

Project of the book [Python Programming Blueprints](https://www.packtpub.com/mapt/book/application_development/9781786468161?utm_source=all%20updates&utm_campaign=a532fdc6a6-Mapt_new_title_releases_25_01_18&utm_medium=email&utm_term=0_c970747b22-a532fdc6a6-169822065&mc_cid=a532fdc6a6&mc_eid=b722ebf882)

## Install

pip install -r requirements.txt

pip install -r requirements_dev.txt

It requeres PhantomJS; you can download it from: http://phantomjs.org/download.html

After downloading it, extract the contents inside the root project directory and rename the folder to phantomjs.

## Today example

python -m weatherterm -u Fahrenheit -a SWXX2372:1:SW -p WeatherComParser -td

```
   33°
    High 0° / Low 22° (Sunny)
    Wind: 46% / Humidity: ENE 7 mph 
```

## Five days examples

python -m weatherterm -u Fahrenheit -a SWXX2372:1:SW -p WeatherComParser -5d

```
    >> Tonight MAR 30
        High 2° / Low 2° (Mostly Clear)
        Wind: NNE 7 mph  / Humidity: 70%

    >> Sat MAR 31
        High 39° / Low 24° (Partly Cloudy)
        Wind: ENE 7 mph  / Humidity: 55%

    >> Sun APR 1
        High 37° / Low 27° (Cloudy)
        Wind: NE 13 mph  / Humidity: 73%

    >> Mon APR 2
        High 38° / Low 22° (AM Snow Showers)
        Wind: NNW 17 mph  / Humidity: 62%

    >> Tue APR 3
        High 42° / Low 27° (Partly Cloudy)
        Wind: WSW 7 mph  / Humidity: 48%

    >> Wed APR 4
        High 42° / Low 34° (Cloudy)
        Wind: SE 9 mph  / Humidity: 73%
```

## For the weekend

python -m weatherterm -u Fahrenheit -a SWXX2372:1:SW -p WeatherComParser -w

```
    >> Sat MAR 31
        High 39° / Low 24° (Partly Cloudy)
        Wind: ENE 7 mph  / Humidity: 55%

    >> Sun APR 1
        High 37° / Low 27° (Cloudy)
        Wind: NE 13 mph  / Humidity: 73%
```

## For help

python -m weatherterm --help