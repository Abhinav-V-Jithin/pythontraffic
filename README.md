I tried a couple of experiments to see if the model in traffic.py is the best one.

(i). When the AI was trained with a model consisting of two convolutional layers, two pooling layers, one hidden dense layer, and one dense output layer, the model achieved an accuracy of 99.58 % and loss = 2.25%

(ii). When the AI was trained with a model consisting of two convolutional, three pooling, one hidden dense layer, and one dense output layer, the model achieved an accuracy of 98.83 % and loss = 5.61 %

(iii). When the AI was trained with a model consisting of two convolutional, three pooling, a dropout, one hidden dense layer, and one dense output layer, the model achieved accuracy of 98.09 % and loss = 8.84 %

				Observations
All the experiments above was found to work, but the best was from (i).

In experiment (ii), the accuracy achieved by the model was found to be reduced, since the pooling layers, made the data became too short that the AI could not learn much from that, but simultaneously misled into wrong learning.

In experiment (iii), the AI had an additional droupout layer, but every neurons might possibly be very important such that they aren't over-relied on them, and the dropout layer caused loss of precision of data learned by the AI.