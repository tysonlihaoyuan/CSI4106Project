# CSI4106Project

Project name: Comparision of Decision Tree and Keras in War Predictions

dataset:

https://www.kaggle.com/umichigan/interstate-wars?fbclid=IwAR008QAZiJ3HeH-P22QxL2pCLPYnIc1T1ci0on68RzYdYMKao8piwHqI-Hk

'interstate.csv', 'intrastate.csv', 'extrastate.csv'

Cassification: 
outcome, intervention

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


method: tree,baseline(log),deep leraning(keras,categorical_crossentropy)  regression, tree baseline(log),deep leraning(keras) classication,

extrastate:
1. claffication:
          output:outcome  input: ini, combat-location, intervention,state-fata, non-stat-fata, side1-code,side2-code
          output:intervention input: ini, combat-location, outcome, state-fata, non-stat-fata, side1-code,side2-code 
2. regresion:  output:state-fata, output: outcome, ini, combat-location, intervention, non-stat-fata, side1-code,side2-code
               output:non-stat-fata, output: outcome, ini, combat-location, intervention, stat-fata, side1-code,side2-code
                    
intrasate:
1. classication
          output: outcome; input: ini, combat-location, side1-code,side2-code, side1_fatalities, side2_fatalities, international_war
          output: international_war; input: ini, combat-location, side1-code,side2-code, side1_fatalities, side2_fatalities, outcome
2. regression
output: side1-fata; input: ini, combat-location, side1-code,side2-code, outcome, international_war, side2 -fata
outout: side2 -fata; input:  ini, combat-location, side1-code,side2-code, outcome, international_war, side1-fata
