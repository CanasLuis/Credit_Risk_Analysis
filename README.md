# Credit_Risk_Analysis
## Purpose
We are seeing one of the most important issues in the real world nowadays, the credit card risk. Banks and financial companies have a lot of trouble when they have to decide whether or not to give a credit card to a client, for one side, it is important to have more clients, and in the other hand, it is important to not lend money to a person that is not willing to pay. As shown, there can be umlimited variables that can be considered when the moment to make a decision arrives, fortunately, we have different supervised machine learning processes we can test.

###Random Forest
![Random_Forest](https://user-images.githubusercontent.com/108499271/206374484-1e03088b-f474-4c64-9477-a97ed164c11d.png)

Random forest method provides us with an accurancy of .65, which is not bad, but we might need a higher number when we are talking about credit cards.

![Random_forest_class report](https://user-images.githubusercontent.com/108499271/206375036-2f77af7f-7013-487b-91d7-3b25b274e742.png)

Precision is .71 for the high risk class, which is, the people that might not pay the credit, that means that the model might identify the majortiy of people with high risk.


###AdaBoost_Clasifier
![AdaBoos_Classifier](https://user-images.githubusercontent.com/108499271/206375530-16b3eaeb-9f3a-49d3-ba84-51d488c87f43.png)

This is not the method I would prefer for this purpose, it has an accurancy level of .5 and the number of high risk identified is .01, which means, a lot of high risk people will be receiving a credit card:

![AdaBoos_Classifier_class report](https://user-images.githubusercontent.com/108499271/206375804-97d770e8-eddb-4bfd-adab-5df39d1b7af5.png)

###OVersampling
this method shows a good accurancy, however the precision is something to be worry about, similar to what was shown in Ada Boost:
![Oversampling](https://user-images.githubusercontent.com/108499271/206376262-e0c14f5f-997f-4453-95e0-0f3daf3e7be1.png)
![Oversampling_class_report](https://user-images.githubusercontent.com/108499271/206376279-a38557c3-bfad-4e1f-9fb8-e2ad7ba8300f.png)


###SMOTE Oversampling
simitar to previous method, this is showing a decent accurancy, however a low precision:

![SMOTE OVERSAMPLING](https://user-images.githubusercontent.com/108499271/206376813-c0155460-dbd6-4ce8-bdb4-ee2dd05788fc.png)
![SMOTE OVERSAMPLING_CLASS](https://user-images.githubusercontent.com/108499271/206376842-f5a2b5ec-1b3f-478e-9f39-5559e25ebade.png)


###Undersampling show even a lower accurancy but precision remains very low for high risk customers.
![Undersampling](https://user-images.githubusercontent.com/108499271/206377136-b03998d0-567a-4aa6-81c8-51e540292f12.png)
![Undersampling_class](https://user-images.githubusercontent.com/108499271/206377153-0362c28b-7533-4f20-81f3-2e3c902b663d.png)


###Over and Under Sampling
![Over and Under Sampling](https://user-images.githubusercontent.com/108499271/206377483-97407400-eb33-40e7-8d8c-4d9a0527470a.png)

![Over and Under Sampling_class](https://user-images.githubusercontent.com/108499271/206377502-858991fe-a5fb-42d5-8623-b2886afeb58d.png)

Accurancy grew a little bit but the precision is still very low. in other cases this might be less important, but financial companies won´t hesitate in rejecting this method in real life. 

##Summary
I would recommend Random Forest algorithm since its the one that showed more precision, also it might identify more high risk clients and be more selective with the clients that can receive a credit card.



