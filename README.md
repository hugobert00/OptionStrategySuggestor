# OptionStrategySuggestor
The language used is Python, the goal of this code is to use a Streamlit interface on which you can give by simple sentence your sentiments on an underlying. For example "wheat futures Z25 will decrease/increase by xx%, or the price will stay between xx and xx, or the volatility will increase/decrease by xx%. Then it gives you a list of strategies.

Strategies are taken from a dictionnary that includes almost more than 150 different option strategies. You can filter strategies at your convinience. For example you can rank them by cost, capped risk/ profit or not... 

Another incoming fonctionality is that you will soon be able to enter your actual positions (option book), then your sentiment and it will give you strategies that are optimized given your actual risk exposure. 

ex : you have an option book with a given risk exposure 
- you say, I want ton increase my delta by... / my gamma or I want to by short theta by xx and it gives you a list of strategies that you can apply
- you say, I think that the volatility on Underlying A will increase by xx% within 2 month, it suggested you the right calendar sprread

Where are the strategies from ? 
- the official CBOE support "How to master option strategies" -
- the classic J.Hull "Options, futures and other derivatives" -
- My own and humble experience -


What is the overall architecture ? 
- a dictionnary with all the strategies available (feel free to insert your own strategies)
- a part that analyses your position
- a part that gives you the right strategies based on your sentiement (strategy selector)
- a main and the streamlit interface is managed in it 

NB : If you are from a top L/S prop shop or hedgefund and reading this (I am looking for an off-cycle internship.. ;) ) 
