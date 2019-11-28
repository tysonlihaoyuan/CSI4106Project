# CSI4106Project

Project name: Comparision of Decision Tree and Keras in War Predictions

dataset:

https://www.kaggle.com/umichigan/interstate-wars?fbclid=IwAR008QAZiJ3HeH-P22QxL2pCLPYnIc1T1ci0on68RzYdYMKao8piwHqI-Hk

'interstate.csv', 'intrastate.csv', 'extrastate.csv'

Cassification: 
outcome, initiation, intervention

Regression:
state_fatalities, nonstate_fatalities


some varibale clearify:
war_type: "1"--> Interstate wars
          "2"--> Colonial war (to maintain control of colony)
          "3"--> Imperial war( to extend empire)
          "4"--> Civil war for central control
          "5"--> Civil war over local issues 
          "6"--> Regional internal war 
          "7"--> Intercommunal war


train group: 0.75
test group: 0.25 

for the multiclass classcification

target file: interstate.csv
target prediction: outcome
target train and analyze: 'side',initiation','combat_location','combat_fatalitie'

for the muticalss regression
target file: interstate.csv
target prediction: 'combat_fatalitie'
target train and analyze: 'side',initiation','combat_location','outcome'

evaluation:
Precision, Recall, and Accuracy.
