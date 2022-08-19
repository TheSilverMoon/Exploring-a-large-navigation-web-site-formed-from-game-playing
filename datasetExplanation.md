# Data Understanding

### Data Files

- [CHQ_trajectory_lengths.csv](http://localhost:8888/edit/MSc/MSc Project/dataset/CHQ_trajectory_lengths.csv)
    - 600 records
    - 6 dimensions(L1, L2, L3, L4, L5, zscore)
    - no missing data
    - inconsistent data formats (text & digit)
    - dataset of City Hero Quest
- [demographics.csv](http://localhost:8888/edit/MSc/MSc Project/dataset/demographics.csv)
    - 600 records
    - 12 dimensions (subID, age, environment, street, city, still_live, city_current, city_current_type, gender, environment_current_binary, environment_binary, education)
    - no missing data
    - inconsistent data formats (text & digit)
    - information of player
    - ★
- [HomeAddressEntropy.csv](http://localhost:8888/edit/MSc/MSc Project/dataset/HomeAddressEntropy.csv)
    - 600 records
    - 3 dimensions (address,environment,entropy_adjusted)
    - no missing data
    - inconsistent data formats (text & digit)
    - entropy adjusted according to address (street level)
- [SHQ_trajectory_lengths.csv](http://localhost:8888/edit/MSc/MSc Project/dataset/SHQ_trajectory_lengths.csv)
    - 600 records
    - 6 dimensions(L1,  L11,  L32,  L42,  L68,  zscore) (Level numbers not in order?)
    - inconsistent data formats (text & digit)
    - dataset of Sea Hero Quest
    - ★

### Feature explanation of Star dataset

#### demographics

- subId: Unique number of users (combined with digit and alphabet)
- age: age of users
- environment: city or suburbs or mix
- street: street address of users
- city : city of users  (Born?)
- still_live: if users are alive or not / if users lived in the same city they were born (More likely)
- city_current: city of users (current stay)
- gender: male or female
- environment_current_binary: City or NonCity (corresponding city_current dimension)
- environment_binary: City or NonCity (corresponding city dimension)
- education: education level users (Secondary, Tertiary)

#### SHQ_trajectory_lengths

- L1: score in Level 1
- L11: score in Level 11
- L32: score in Level 32
- L42: score in Level 42
- L68: score in Level 68
- zscore: weighted score of users(rules unknown)

### Large Dataset
#### Explanation of features
- uuid: Unique User Id
- stored_at: When the data is stored in server
- duration: Time during this level
- previous_attemps: Previous attempt times
- platform: ANDROID or IOS
- app_verstion: version of SHQ
- map_view_duration: Time of viewing the map before start the game
- events: preset landmark or flags, only the visible flag is the target
- player：Trajectory of the boat in the game

