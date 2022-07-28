# TimeSeriesMomentumTradingStrategy

This again uses the Strategies class as the basis for this strategy as seen in my BuyandHold algorithm.

In this strategy, a Time Series Momentum Strategy is Created.

This takes a positions of every asset in the given basket.

If an asset have a negative historic return, then a short position is taken and if it has a positive historic return then a long position is taken.

The lookback period for which returns are calcualted is the previous t days.

We also only adjust the portfolio weights every q days. Note the first date we can calculate weights will be on date t so we aim to adjust the portfolio weights every q days after this.

Then aim to normalise weights by ensuring sum of the aboslute values of all weights on any given date is 1.
