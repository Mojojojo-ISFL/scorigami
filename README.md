# scorigami
Data and analysis/visualization code for ISFL and DSFL scorigami.

Data dictionaries:
This folder includes two main data files. The first, ISFL_scorigami.csv, includes all games played in ISFL/NSFL league history. The second, DSFL_scorigami.csv, includes the same data for all games played in DSFL history. Data was scraped from the forum index "Weekly Results" page for each season of each league. 

These datasets have the games as rows and the following variables as columns: the season number (Season), week number (Week), winning team code (Team_won) and final score (FinalScore_won), losing team code (Team_lost) and final score (FinalScore_lost), win type (WinType = HOME, AWAY, or TIE), and score differential (PointDiff) for all regular season and playoff games. Pre-season games are not included. 

Team codes for the Team_won and Team_lost variables are:
ISFL
  AUS = Austin Copperheads
  AZ = Arizona Outlaws
  BAL = Baltimore Hawks
  CHI = Chicago Butchers
  COL = Colorado Yeti
  HON = Honolulu Hahalua
  LV = Las Vegas Legion
  NO = New Orleans Second Line
  OCO = Orange County Otters
  PHI = Philadelphia Liberty
  SAR = Sarasota Sailfish
  SJS = San Jose SaberCats
  YKW = Yellowknife Wraiths
DSFL
  CHI = Chicago Blues
  DAL = Dallas Birddogs
  KC = Kansas City Coyotes
  LON = London Royals
  MB = Myrtle Beach Buccaneers
  MIN = Minnesota Grey Ducks
  NOR = Norfolk Seawolves
  PB = Palm Beach Solar Bears
  POR = Portland Pythons
  SA = San Antonio Marshalls 
  TIJ = Tijuana Luchadores

Note for ISFL_scorigami.csv: playoff byes that appear in the index but were simulated until the bye team won were excluded from the database. These were determined based on best overall record going into the playoff bracket for seasons 16 through 24. 

One additional dataset is included, ImpossibleScores.csv, which is a simple list of score pairs that are impossible, either because they require scoring a single point by itself or would require the losing team to score more than the winning team. These are generated for visualization purposes only.
