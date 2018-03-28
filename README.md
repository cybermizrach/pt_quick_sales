# Profit Trailer Settings: Quick Sales Strategy
Settings for Profit Trailer and PTMagic. This group of settings is heard towards a quick rate of sales and purchases with sell values around 1% each.

# FAQ
Q: Will this work with BTC?
A: Yes. You will need to update the below two properties in your PAIRS.properties.
	market = BTC
	ALL_max_trading_pairs = ???

Q: Are you working on anything new?
A: Yes! I have been collaborating with a few other interested individuals who shared a very insightful article with me. In this setup, the goal will be to go after only well-behaving pairs that allow profits of 5-10% for each pair. DCA levels will be deep. The settings.analyzer file will be much smaller. The outlook will be DAYS and not hours. The number of concurrently running pairs will hopefully end up being double of the current setup. I started testing this on March 23rd and probably won't release settings for this until April, pending the results. To learn more, visit https://medium.com/@wisepapertiger/profit-trailer-bitcoin-cryptobot-that-makes-lots-of-money-bitcoin-currency-trading-c4f618e048fc

Q: What should I set ALL_max_trading_pairs to?
A: You'll need to determine what your max trading pairs is based on your comfort levels, balance, DCA levels, and risk acceptance. Let's say you have a good ETH balance like 2 ETH....in this case I'd trade more pairs, instead of larger pairs. This will pool your risk among many pairs. If you have a lower balance, then clearly you'll only be able to run less pairs. The true limiting factor on the number of pairs you run is your DCA setup. The current DCA setup is "shallow" and I'm currently testing a much greater depth of DCAs. For the time being, recommend you check out this file provided by JB, a member of the Crypto Gnome team: https://docs.google.com/spreadsheets/d/1RAh-xjqsOQITBZmaf2ZTbPqq2aqjyKwF_kJuesaMFPc/edit?usp=sharing

Q: Why do you use ALL_max_cost_percentage instead of ALL_max_cost?
A: Bottom line up front: to make sure you're compounding. Longer explanation: if you use percentage, then each time you buy it will take into account previous gains/losses. If you're making gains, subsequent buys will be larger and will in theory return greater net gains.

Q: Why are so many pairs in Sell Only Mode?
A: This group of settings was designed to get in and out of pairs that show favorable behavior. It avoids anything that can be risky like downtrends and pumps. Unfortunately, a lot of pairs just don't make the cut. If you want to trade pairs that are downtrending, remove the downtrending setting. Another option is to change the ALL_buy_strategy to something like LOWBB or EMAGAIN. I tried this and wasn't pleased with the results because the whole point of these settings is to get IN AND OUT as quickly as possible. If you want look at holding a pair for days at a time, then this setup might not work for you. Or, you'll need to adjust your DCA levels for a much greater level of depth.
