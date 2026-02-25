# Awesome Sports Betting [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of tools, APIs, datasets, libraries, models, and resources for sports betting, handicapping, and quantitative sports analysis.

Maintained by [Ian Alloway](https://github.com/ianalloway). Contributions welcome!

---

## Contents

- [Odds APIs](#odds-apis)
- [Datasets](#datasets)
- [Python Libraries](#python-libraries)
- [R Libraries](#r-libraries)
- [ML Models & Papers](#ml-models--papers)
- [Kelly Criterion & Bankroll Management](#kelly-criterion--bankroll-management)
- [CLV & Line Shopping](#clv--line-shopping)
- [DFS Tools](#dfs-tools)
- [Books](#books)
- [Podcasts](#podcasts)
- [Communities](#communities)
- [Platforms & Sportsbooks](#platforms--sportsbooks)
- [Related Awesome Lists](#related-awesome-lists)
- [Contributing](#contributing)

---

## Odds APIs

*APIs for retrieving live and historical odds across sportsbooks.*

- [The Odds API](https://the-odds-api.com/) - Aggregated odds from 70+ bookmakers worldwide with a generous free tier. Supports NFL, NBA, MLB, NHL, soccer, and more.
- [Sportradar](https://sportradar.com/) - Enterprise-grade sports data provider powering the NFL, NBA, MLB, and NASCAR with official league data feeds.
- [Betfair Exchange API](https://developer.betfair.com/) - Programmatic access to the world's largest betting exchange, including market data, placing bets, and streaming prices.
- [Odds API (odds-api.com)](https://odds-api.com/) - Real-time and historical odds comparison API covering major US and European sportsbooks.
- [BetBrain API](https://www.betbrain.com/) - Odds comparison data from 200+ bookmakers across 30+ sports.
- [Pinnacle API](https://www.pinnacle.com/en/api) - Direct API access to Pinnacle's sharp lines, widely regarded as the market benchmark.
- [Kambi API](https://kambi.com/) - B2B sportsbook technology provider powering DraftKings, Unibet, and others.
- [DraftKings API](https://sportsbook.draftkings.com/) - Unofficial endpoints for retrieving DraftKings odds and market data.
- [FanDuel API](https://sportsbook.fanduel.com/) - Unofficial endpoints for FanDuel sportsbook odds retrieval.
- [Betfair Historical Data](https://historicdata.betfair.com/) - Tick-by-tick historical exchange data for backtesting trading strategies.
- [SportsDataIO](https://sportsdata.io/) - Real-time and historical sports data APIs for odds, scores, projections, and player stats.
- [OddsPortal](https://www.oddsportal.com/) - Historical odds archive and comparison tool across hundreds of bookmakers.

## Datasets

*Publicly available datasets for sports analytics and model building.*

### Multi-Sport

- [Kaggle Sports Datasets](https://www.kaggle.com/datasets?search=sports+betting) - Community-contributed datasets covering betting lines, game results, and player stats.
- [Sports Reference](https://www.sports-reference.com/) - The gold standard for historical sports statistics across MLB, NFL, NBA, NHL, and college sports.
- [FiveThirtyEight Data](https://github.com/fivethirtyeight/data) - Open datasets from FiveThirtyEight including ELO ratings, game predictions, and historical forecasts.

### NFL

- [nflverse/nfldata](https://github.com/nflverse/nfldata) - Comprehensive NFL play-by-play, roster, and schedule data updated weekly during the season.
- [nflverse/nflfastR-data](https://github.com/nflverse/nflfastR-data) - Pre-cleaned NFL play-by-play data with EPA, WPA, and CPOE metrics going back to 1999.
- [Pro Football Reference](https://www.pro-football-reference.com/) - Complete NFL historical statistics including game logs, advanced stats, and draft data.
- [Kaggle NFL Big Data Bowl](https://www.kaggle.com/c/nfl-big-data-bowl-2024) - Annual competition with NFL Next Gen Stats tracking data for player movement analysis.
- [Aussie Rules NFL Dataset](https://www.kaggle.com/datasets/tobycrabtree/nfl-scores-and-betting-data) - NFL scores and betting data including spreads and over/unders from 1966 to present.

### NBA

- [Basketball Reference](https://www.basketball-reference.com/) - Comprehensive NBA, ABA, and WNBA statistical database with advanced metrics.
- [NBA Stats API](https://www.nba.com/stats/) - Official NBA stats endpoint providing player tracking, shot charts, and advanced analytics.
- [Kaggle NBA Dataset](https://www.kaggle.com/datasets/nathanlauga/nba-games) - Historical NBA game data with team stats, rankings, and game outcomes.
- [NBA Shot Charts Dataset](https://github.com/swar/nba_api) - Programmatic access to shot-level data from stats.nba.com.
- [NBA Betting Dataset (Kaggle)](https://www.kaggle.com/datasets/ehallmar/nba-historical-stats-and-betting-data) - NBA historical stats merged with betting lines and totals.

### MLB

- [Lahman Baseball Database](https://www.seanlahman.com/baseball-archive/statistics/) - The most comprehensive open baseball database covering stats from 1871 to present.
- [Retrosheet](https://www.retrosheet.org/) - Play-by-play data for every MLB game going back to 1921, including event files.
- [Statcast Data (Baseball Savant)](https://baseballsavant.mlb.com/) - MLB pitch-level and batted-ball tracking data with exit velocity, launch angle, and spin rate.
- [pybaseball Data](https://github.com/jldbc/pybaseball) - Python scraper for FanGraphs, Baseball Reference, and Statcast data.

### Soccer

- [football-data.co.uk](https://www.football-data.co.uk/) - Historical match results and betting odds for 20+ soccer leagues going back to the 1990s.
- [FBref](https://fbref.com/) - Advanced soccer statistics powered by StatsBomb data for major leagues worldwide.
- [Transfermarkt](https://www.transfermarkt.com/) - Player valuations, transfer history, and squad information for soccer leagues globally.
- [Open Football Data](https://github.com/openfootball) - Free open public domain football data covering leagues, cups, and national teams.
- [European Soccer Database (Kaggle)](https://www.kaggle.com/datasets/hugomathien/soccer) - 25,000+ matches from 11 European leagues with player attributes from FIFA video games.

### Other Sports

- [Tennis Abstract](https://www.tennisabstract.com/) - Match-by-match historical tennis results with Elo ratings and serve statistics.
- [UFC Stats](http://ufcstats.com/) - Official UFC fight statistics including striking, grappling, and fight outcomes.
- [Hockey Reference](https://www.hockey-reference.com/) - Complete NHL statistical database with game logs and advanced metrics.

## Python Libraries

*Python packages for data retrieval, analysis, and model building.*

### Data Retrieval

- [nba_api](https://github.com/swar/nba_api) - Python client for the NBA Stats API providing access to player, team, and game data from stats.nba.com.
- [nfl_data_py](https://github.com/cooperdff/nfl_data_py) - Python wrapper for nflverse data, providing easy access to play-by-play, roster, and schedule data.
- [sportsipy](https://github.com/roclark/sportsipy) - Pull clean and structured data from Sports Reference for MLB, NBA, NFL, NHL, and college sports.
- [pybaseball](https://github.com/jldbc/pybaseball) - Scrape Baseball Reference, FanGraphs, and Statcast data with simple Python function calls.
- [sportsreference](https://github.com/roclark/sportsreference) - Pull data from Sports Reference sites for multiple sports with a Pythonic API.
- [basketball_reference_scraper](https://github.com/vishaalagartha/basketball_reference_scraper) - Lightweight scraper for Basketball Reference data including box scores and player stats.
- [sportypy](https://github.com/sportsdataverse/sportypy) - Generate scaled, accurate sports field and court visualizations in Python.
- [cfbd](https://github.com/CFBD/cfbd-python) - Python client for the College Football Data API, providing access to play-by-play data and recruiting.
- [hockey_scraper](https://github.com/HarryShomer/Hockey-Scraper) - Scrape NHL play-by-play, shift, and schedule data from NHL.com and ESPN.

### Analysis & Modeling

- [pandas](https://github.com/pandas-dev/pandas) - The backbone of tabular data manipulation in Python; essential for cleaning and transforming sports data.
- [scikit-learn](https://github.com/scikit-learn/scikit-learn) - Machine learning library with classification, regression, and clustering algorithms for building prediction models.
- [XGBoost](https://github.com/dmlc/xgboost) - Gradient boosting framework frequently used in sports prediction competitions for its speed and accuracy.
- [LightGBM](https://github.com/microsoft/LightGBM) - Fast gradient boosting framework from Microsoft, efficient for large-scale sports datasets.
- [PyTorch](https://github.com/pytorch/pytorch) - Deep learning framework used for building neural network-based sports prediction models.
- [statsmodels](https://github.com/statsmodels/statsmodels) - Statistical modeling library for regression analysis, time series, and hypothesis testing on sports data.
- [optuna](https://github.com/optuna/optuna) - Hyperparameter optimization framework for tuning sports prediction model parameters.
- [PuLP](https://github.com/coin-or/pulp) - Linear programming library useful for DFS lineup optimization and bankroll allocation.

## R Libraries

*R packages for sports data and analytics.*

- [nflfastR](https://github.com/nflverse/nflfastR) - Fast scraping and cleaning of NFL play-by-play data with EPA and CPOE models built in.
- [nflreadr](https://github.com/nflverse/nflreadr) - Minimal, fast package to read nflverse data releases without needing nflfastR.
- [hoopR](https://github.com/sportsdataverse/hoopR) - Access NBA and men's college basketball data from ESPN and the NBA Stats API.
- [wehoop](https://github.com/sportsdataverse/wehoop) - Access WNBA and women's college basketball play-by-play data.
- [baseballr](https://github.com/BillPetti/baseballr) - Scrape MLB data from Statcast, FanGraphs, and Baseball Reference directly into R.
- [cfbfastR](https://github.com/sportsdataverse/cfbfastR) - Access college football play-by-play data and recruit rankings.
- [worldfootballR](https://github.com/JaseZiv/worldfootballR) - Extract soccer data from FBref, Transfermarkt, Understat, and FotMob.
- [hockeyR](https://github.com/danmorse314/hockeyR) - Load and clean NHL play-by-play data with expected goals models.
- [BradleyTerry2](https://cran.r-project.org/package=BradleyTerry2) - Fit Bradley-Terry paired comparison models, commonly used for team strength estimation.

## ML Models & Papers

*Machine learning approaches, published models, and academic papers on sports prediction.*

### Models & Frameworks

- [FiveThirtyEight ELO Ratings](https://fivethirtyeight.com/methodology/how-our-nfl-predictions-work/) - Nate Silver's ELO-based prediction system for NFL, NBA, and MLB with publicly documented methodology.
- [FiveThirtyEight RAPTOR](https://fivethirtyeight.com/features/how-our-raptor-metric-works/) - Player-level plus-minus model combining box score and tracking data for NBA predictions.
- [Microsoft Research SportsCastr](https://www.microsoft.com/en-us/research/project/sports-analytics/) - Microsoft's sports analytics research including real-time prediction models.
- [Google DeepMind Football](https://github.com/google-research/football) - Reinforcement learning environment for football (soccer) strategy research.
- [NFL Next Gen Stats](https://nextgenstats.nfl.com/) - AWS-powered tracking analytics providing completion probability, expected rushing yards, and win probability.
- [Inpredictable](https://www.inpredictable.com/) - Publicly available NFL and NBA win probability and ELO models with transparent methodology.
- [ESPN BPI](https://www.espn.com/college-football/bpi) - ESPN's team strength and game prediction model using Bayesian methods.
- [KenPom](https://kenpom.com/) - Widely respected college basketball efficiency ratings used for March Madness predictions.

### Academic Papers

- [Beating the Bookies with Their Own Numbers](https://arxiv.org/abs/1710.02824) - Demonstrates profitable soccer betting strategies using bookmaker consensus odds.
- [Predicting Football Results Using Machine Learning](https://arxiv.org/abs/1806.07366) - Comprehensive comparison of ML techniques for European football match prediction.
- [A Machine Learning Framework for Sport Result Prediction](https://www.sciencedirect.com/science/article/pii/S2210832717301485) - Framework for evaluating various ML approaches to sports prediction.
- [Deep Learning for Sports Outcome Prediction](https://arxiv.org/abs/1901.03717) - Application of LSTM and recurrent neural networks to sequential sports data.
- [Applying Machine Learning to NBA Data](https://arxiv.org/abs/2002.03043) - Predicting NBA game outcomes using ensemble methods and player-level features.
- [Dixon-Coles Model](https://www.jstor.org/stable/2986290) - Foundational paper on modeling soccer scores with a bivariate Poisson distribution and dependence parameter.
- [Massey Ratings](https://www.masseyratings.com/) - College sports ranking system based on solving systems of linear equations from game results.
- [Glicko Rating System](http://www.glicko.net/glicko.html) - Rating system extending ELO with rating deviation and volatility, applicable to sports prediction.

## Kelly Criterion & Bankroll Management

*Tools and resources for optimal bet sizing and bankroll management.*

- [kelly-js](https://github.com/ianalloway/kelly-js) - Lightweight JavaScript implementation of Kelly Criterion for calculating optimal bet sizes, supporting fractional Kelly and simultaneous bets.
- [Kelly Criterion Calculator (Wizard of Odds)](https://wizardofodds.com/gambling/kelly-criterion/) - Online calculator for determining optimal bet fractions based on edge and odds.
- [PyKelly](https://github.com/WillianFuworworker/PyKelly) - Python implementation of the Kelly Criterion with support for multiple simultaneous outcomes.
- [Kelly Criterion (Wikipedia)](https://en.wikipedia.org/wiki/Kelly_criterion) - Comprehensive mathematical overview of the Kelly Criterion with proofs and examples.
- [Fractional Kelly Strategies](https://www.pinnacle.com/en/betting-articles/Betting-Strategy/the-kelly-criterion/TMB7KDBKX4CF3GVY) - Pinnacle's guide to using fractional Kelly for more conservative bankroll management.
- [Staking Plans Comparison](https://www.football-data.co.uk/staking.php) - Empirical comparison of Kelly, flat, and proportional staking plans across historical soccer data.

### Books on Bankroll Management

- [Fortune's Formula by William Poundstone](https://www.goodreads.com/book/show/186124.Fortune_s_Formula) - The story of the Kelly Criterion, from information theory to Wall Street to gambling.
- [The Kelly Capital Growth Investment Criterion](https://www.goodreads.com/book/show/11685875-the-kelly-capital-growth-investment-criterion) - Collected academic papers on Kelly strategies edited by MacLean, Thorp, and Ziemba.

## CLV & Line Shopping

*Tools for tracking closing line value and comparing odds across sportsbooks.*

- [OddsJam](https://oddsjam.com/) - Real-time odds comparison, positive EV finder, and CLV tracker across 50+ sportsbooks.
- [Pinnacle](https://www.pinnacle.com/) - The sharpest sportsbook in the world; Pinnacle closing lines are the industry benchmark for CLV measurement.
- [DarkHorse Odds](https://www.darkhorseodds.com/) - Odds comparison and arbitrage finder for US-legal sportsbooks.
- [OddsShopper](https://www.oddsshopper.com/) - Line shopping tool with conversion calculators, hold percentages, and best-odds highlighting.
- [Unabated](https://unabated.com/) - Professional-grade line shopping, no-vig fair odds calculator, and CLV tracking dashboard.
- [BetStamp](https://betstamp.app/) - Bet tracking app with automatic CLV calculation, ROI analysis, and odds comparison.
- [Rebel Betting](https://www.rebelbetting.com/) - Value betting and sure betting (arbitrage) finder covering international sportsbooks.
- [Odds Shark](https://www.oddsshark.com/) - Free odds comparison and historical line movement charts for major US sports.
- [Action Network](https://www.actionnetwork.com/) - Odds comparison, public betting percentages, and sharp money indicators.
- [SharpSide](https://sharpside.app/) - Bet tracking and analytics platform with CLV monitoring and bankroll visualization.

## DFS Tools

*Daily fantasy sports optimization and research tools.*

- [FantasyLabs](https://www.fantasylabs.com/) - Data-driven DFS research platform with player models, ownership projections, and correlation tools.
- [SaberSim](https://www.sabersim.com/) - Lineup optimizer using game simulations and projected ownership for GPP tournament strategy.
- [RotoGrinders](https://rotogrinders.com/) - DFS community with free projections, articles, lineup tools, and the GrindersLive show.
- [DraftKings Optimizer (LineStarApp)](https://www.linestarapp.com/) - Free DFS lineup generator and optimizer for DraftKings and FanDuel.
- [FantasyCruncher](https://www.fantasycruncher.com/) - Advanced lineup optimizer with late-swap support, multi-entry tools, and stacking features.
- [Daily Fantasy Nerd](https://dailyfantasynerd.com/) - Projections aggregator and optimizer that combines multiple expert projection sources.
- [Stokastic](https://stokastic.com/) - DFS projections, ownership models, and optimal lineup construction tools.
- [AwesemoDFS](https://www.awesemo.com/) - Premium DFS projections with course-fit models for golf and positional rankings for all sports.

## Books

*Essential reading for sports bettors, from beginner to advanced.*

### Quantitative & Strategy

- [Sharp Sports Betting by Stanford Wong](https://www.goodreads.com/book/show/254218.Sharp_Sports_Betting) - A classic reference on sports betting mathematics covering closing line value, money management, and market theory.
- [Calculated Bets by Steven Skiena](https://www.goodreads.com/book/show/2266928.Calculated_Bets) - Computer science professor documents building an automated prediction system for jai alai, applicable to any sport.
- [Trading Bases by Joe Peta](https://www.goodreads.com/book/show/15811521.Trading_Bases) - A Wall Street trader applies financial modeling techniques to MLB betting with entertaining narrative.
- [Mathletics by Wayne Winston](https://www.goodreads.com/book/show/6739521.Mathletics) - How math and analytics are used across major sports for roster construction, in-game strategy, and prediction.
- [The Signal and the Noise by Nate Silver](https://www.goodreads.com/book/show/13588153.The_Signal_and_the_Noise) - Broad exploration of prediction science with dedicated chapters on sports forecasting and poker.
- [Weighing the Odds in Sports Betting by King Yao](https://www.goodreads.com/book/show/1186139.Weighing_the_Odds_in_Sports_Betting) - Practical guide covering middle plays, scalps, steam moves, and the math behind sports betting markets.
- [Statistical Sports Models in Excel by Andrew Mack](https://www.goodreads.com/book/show/42363484-statistical-sports-models-in-excel) - Step-by-step guide to building prediction models in Excel for sports bettors.

### Market & Behavioral

- [The Logic of Sports Betting by Ed Miller & Matthew Davidow](https://www.goodreads.com/book/show/52348422-the-logic-of-sports-betting) - Modern guide to understanding how sportsbooks set lines and where bettors can find edges.
- [Squares & Sharps, Suckers & Sharks by Joseph Buchdahl](https://www.goodreads.com/book/show/29633789-squares-sharps-suckers-sharks) - Deep dive into the psychology and statistics of sports betting markets.
- [The Drunkard's Walk by Leonard Mlodinow](https://www.goodreads.com/book/show/2272880.The_Drunkard_s_Walk) - Exploration of randomness and probability that gives essential context for understanding sports outcomes.
- [Thinking, Fast and Slow by Daniel Kahneman](https://www.goodreads.com/book/show/11468377.Thinking_Fast_and_Slow) - Foundational work on cognitive biases directly applicable to avoiding common betting mistakes.
- [Superforecasting by Philip Tetlock](https://www.goodreads.com/book/show/23995360.Superforecasting) - Research on what makes accurate forecasters, with lessons directly applicable to handicapping.

## Podcasts

*Podcasts covering sports betting strategy, analysis, and news.*

- [Behind the Bets (ESPN)](https://www.espn.com/espnradio/podcast/archive/_/id/17467828) - Doug Kezirian's show covering the Las Vegas sports betting scene with sharp analysis.
- [Beating the Book](https://www.beatingthebook.com/) - Gill Alexander's weekly podcast focused on NFL sides, totals, and market analysis.
- [The Athletic Gambling Podcast](https://theathletic.com/podcast/153-the-athletic-gambling-show/) - Data-driven betting discussion across multiple sports from The Athletic's staff.
- [You Better You Bet (VSiN)](https://www.vsin.com/show/you-better-you-bet/) - Nick Kostos and Ken Barkley cover daily sports betting markets with a conversational approach.
- [Bet the Process](https://www.spanky.com/) - Spanky's data-driven approach to NFL and NBA betting with transparent record-keeping.
- [The Favorites (FanDuel)](https://www.fanduel.com/theduel/tag/the-favorites-podcast) - FanDuel's betting strategy podcast covering lines, props, and market movements.
- [Circles Off](https://circlesoff.com/) - Podcast about the sports betting industry covering market dynamics, technology, and regulation.
- [The Ringer Gambling Show](https://www.theringer.com/gambling-show) - Bill Simmons' network explores betting angles across NFL, NBA, and college sports.
- [Pinnacle Podcast](https://www.pinnacle.com/en/betting-articles/podcast) - Educational content on betting strategy, market efficiency, and value finding from the sharpest book.
- [Edge (with Andrew Brandt)](https://podcasts.apple.com/us/podcast/the-business-of-sports-with-andrew-brandt/id1492506470) - Business side of sports including the growing legal sports betting industry.

## Communities

*Online communities for discussion, strategy, and sharp betting content.*

### Reddit

- [r/sportsbook](https://www.reddit.com/r/sportsbook/) - The largest sports betting subreddit with daily pick threads, strategy discussion, and market analysis.
- [r/sportsbetting](https://www.reddit.com/r/sportsbetting/) - General sports betting community for sharing picks, parlays, and betting experiences.
- [r/sportscontests](https://www.reddit.com/r/sportscontests/) - Organized prediction contests with leaderboards and transparent record-keeping.
- [r/NFLBetting](https://www.reddit.com/r/NFLBetting/) - Dedicated NFL betting discussion including spreads, totals, and player props.
- [r/sportsbookextra](https://www.reddit.com/r/sportsbookextra/) - Supplementary sports betting subreddit for additional discussion and analysis.

### Discord & Forums

- [Discord: Unabated Community](https://unabated.com/) - Professional betting community focused on CLV, market theory, and quantitative approaches.
- [Discord: OddsJam Community](https://oddsjam.com/) - Active Discord for positive EV and arbitrage discussion with automated alerts.
- [Covers.com Forum](https://www.covers.com/forum) - One of the oldest sports betting forums with active discussion across all major sports.
- [SBR Forum (SportsbookReview)](https://www.sportsbookreview.com/forum/) - Long-running forum with sportsbook reviews, picks, and industry discussion.

### Twitter / X Accounts

- [@PlusEVAnalytics](https://twitter.com/PlusEVAnalytics) - Quantitative sports betting content focused on positive expected value strategies.
- [@CaptainJackBets](https://twitter.com/CaptainJackBets) - Sharp bettor sharing insights on market movements and betting strategy.
- [@MarkKafalas](https://twitter.com/MarkKafalas) - Former Pinnacle employee sharing sportsbook and sharp market analysis.
- [@spanaboredMTL](https://twitter.com/spanaboredMTL) - Data-driven bettor sharing transparent plays and model output.
- [@ActionNetworkHQ](https://twitter.com/ActionNetworkHQ) - Breaking odds, line moves, public betting percentages, and market analysis.

## Platforms & Sportsbooks

*Major sportsbooks and platforms with API access or notable features for serious bettors.*

### Sharp-Friendly / API Access

- [Pinnacle](https://www.pinnacle.com/) - The gold standard for sharp bettors; lowest margins, highest limits, and doesn't limit winners.
- [Betfair Exchange](https://www.betfair.com/) - Peer-to-peer betting exchange allowing lay bets and in-play trading with exchange API access.
- [Circa Sports](https://www.circasports.com/) - Las Vegas-based sportsbook known for high limits and welcoming sharp action.
- [Bookmaker.eu](https://www.bookmaker.eu/) - Offshore sportsbook respected for high limits and tolerance of winning players.
- [BetOnline](https://www.betonline.ag/) - International sportsbook with competitive lines and prop markets.

### US Legal Sportsbooks

- [DraftKings Sportsbook](https://sportsbook.draftkings.com/) - Major US sportsbook with extensive prop markets, live betting, and same-game parlays.
- [FanDuel Sportsbook](https://sportsbook.fanduel.com/) - Leading US sportsbook known for competitive odds on main markets and user-friendly interface.
- [BetMGM](https://sports.betmgm.com/) - Full-featured sportsbook backed by MGM Resorts with a wide range of markets.
- [Caesars Sportsbook](https://www.caesars.com/sportsbook-and-casino) - Major US sportsbook with the Caesars Rewards loyalty integration.
- [PointsBet](https://pointsbet.com/) - Innovative sportsbook featuring PointsBetting where payouts scale with margin of victory.
- [BetRivers](https://www.betrivers.com/) - US sportsbook from Rush Street Interactive available in multiple states.
- [Hard Rock Bet](https://www.hardrock.bet/) - Sportsbook from the Seminole Tribe of Florida expanding to additional states.

## Related Awesome Lists

*Other curated lists that complement sports betting research.*

- [awesome-machine-learning](https://github.com/josephmisiti/awesome-machine-learning) - Comprehensive list of ML frameworks, libraries, and software across all languages.
- [awesome-quant](https://github.com/wilsonfreitas/awesome-quant) - Curated list of libraries, packages, and resources for quantitative finance. Many tools transfer directly to sports betting.
- [awesome-deep-learning](https://github.com/ChristosChristofidis/awesome-deep-learning) - Deep learning tutorials, projects, and resources applicable to sports prediction models.
- [awesome-datascience](https://github.com/academic/awesome-datascience) - Data science resources including tools, tutorials, and communities relevant to sports analytics.
- [awesome-python-data-science](https://github.com/krzjoa/awesome-python-data-science) - Python libraries for data science including visualization, NLP, and ML tools.
- [awesome-r](https://github.com/qinwf/awesome-R) - Curated list of R packages and tools useful for statistical sports modeling.
- [awesome-football](https://github.com/planetopendata/awesome-football) - Open data, tools, and resources for soccer (football) analytics.
- [awesome-sports-analytics](https://github.com/onlyjus/awesome-sports-analytics) - Curated list of sports analytics resources, tools, and communities.

## Contributing

Contributions are welcome! Please read the [contributing guidelines](CONTRIBUTING.md) first.

---

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Ian Alloway](https://github.com/ianalloway) has waived all copyright and related or neighboring rights to this work.
