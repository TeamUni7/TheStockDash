# The Stock Dash

This project is a model dashboard for Stock Value Analysis. The Analysis include predicting values of stock market indexes in the near future, analysing historical data of the indexes graphically for any given period of time in period, crawling the live value of stock indexes and storing these values in database for future analysis.
The dashboard is a web app developed using Django at the backend and Javascript,Jquery and D3 at the frontend.In broader terms,the project consists of following parts:

#### 1.Live Stock Values : 
This division performs the function of web crawling for live value of NIFTY,SENSEX,GOLD(24 carat) and NASDAQ every minute and displays it. Also every day at 02:00 AM the crawled data is stored in the database in a JSON file.The web crawling is done using .get function of Jquery Ajax so that data can be stored without page refresh.

#### 2.Historic Data Values : 
This division performs the function of showing the data stored in database in a graphical format for analysis. The values of various indices are represented using line graph. Here the programs loads the data from database and then on the basis of this data draws the graph using Data Driven Documents(D3.js).The graph can also be zoomed to show the historical graph on for any given interval of date.

#### 3.Predict Stock Values : 
The value of stock indices stored in the database and used for creating graph can be used to predict the future values of stock. This division contains date input where one can enter the date at which we need to predict the stock values. For the given date the values of SENSEX,GOLD and NASDAQ is calculated using Linear Regression and based upon theses calculated values the value of NIFTY is calculated using Multi Regression. These calculations are performed using Javascript and Jquery.


## Getting Started

Just download the whole repository in zip format ,unzip it. 
### Prerequisites

#### Concepts

```
1. Javascript, Jquery, D3, Django, HTML and CSS.
2. Fundamental of Linear Regression, Multi Regression and Ajax.
```
#### Software and Tools

```
1. Python IDE with pre installed Django package to set up a server atmosphre.(I used PyCharm).
2. Proper internet connection as web crawling can't be done without it.
```
### Installing

Download all the files of repository. Create a project in IDE and add the files of the repository to the project.Now run the command prompt and go the directory of the repository. Now to establish the server execute the following command:
```
python manage.py runserver
```
This would establish the django server atmosphere. To edit the code open the required file of the project in the IDE.

## Authors

* **Nabh Choudhary** - *Initial work* - [grandpriest](https://github.com/grandpriest).

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details
![Alt text](https://github.com/grandpriest/Spoj-Teller/blob/master/Spoj%20Teller/Screenshot%20(47).png)
## Acknowledgments
* The project was done under the guidance of **DR. ABHIJIT MUSTAFI** 
,Associate Professor , Computer Science and Engg ,BIT Mesra.
* The Code Segment of Stock repository of [anudeexCR7](https://github.com/anudeexCR7) was used.
