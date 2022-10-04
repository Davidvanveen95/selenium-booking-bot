

# What is Booking.com?

Booking.com is an online travel agency for lodging reservations & other travel products. It provides online reservation services; acting as an intermediary (agent) between guests wanting to make an accommodation reservation and hotels, property or temporary/holiday rental owners.

# What does this bot do?

This bot allows the user to automate the process of searching and filtering the best deals in Booking.com. Once the bot has finished running it will output a table in the terminal showing the 25 best deals for your chosen destination, based on price and customer ratings.

## Preparing the environment:

- You need python installed
- You need an IDE, for example PyCharm or Visual Studio Code
- Check your Chrome browser version by typing "chrome://version" in the search bar.
- Download the Chromedriver executable file from: https://chromedriver.storage.googleapis.com/index.html Make sure to download the applicable file according to your Chrome browser version.
- Move the downloaded zip file into your C: Drive, and extract the file.
- Copy and paste the file path into the PATH variable located inside the constants.py file.

## How to use this bot:

- In the main.py file you will find the following fields:

```py
bot.change_currency(currency="USD")
bot.select_place_to_go("Amsterdam")
bot.select_date(check_in_date="2022-09-28", check_out_date="2022-10-03")
bot.select_adults(2)
bot.select_children(2)
bot.select_rooms(2)
```

For each one of the previous fields, you can change the value between parenthesis() according to your desired search results.

Example: for the first option you could change the desired currency from "USD" to "CRC" or "EU".

In the booking.py file you will find the apply_filtrations method with the following field:

```py
filtration.apply_star_ratings(3, 4, 5)
```

In this field you can choose the desired star ratings, using comma-space separations if more than one.

To run the code, go to your command line and change to the directory that contains the main.py file.

Then run the following command: `python main.py`

The chrome browser will open up, and the browser will be run automatically. Finally, you can visit your terminal, where a table will be printed out containing a list of the best deals according to the parameters that you decided to set.
