## Datasheet

**Motivation**: The eight datasets come from a Black-Box Optimization challenge. Each function started with a fixed set of base observations, and one new point was added each week. That weekly point was my query for the function.

**Composition**: The eight datasets use features scaled to [0,1]. Each feature vector represents a point in a [0,1]^k space, where k is the number of features for that function. All datasets are complete with no missing values. The datasets currently have the following format:

Function 1: (19,3) 

Function 2: (19,3)

Function 3: (24,4)

Function 4: (39,5)

Function 5: (29,5)

Function 6: (29,6)

Function 7: (39,7)

Function 8: (49,9)

where the last column is the output and the remaining columns are features.

**Collection process**: My queries were generated primarily using Bayesian optimization. For Functions 1 and 2, the queries also incorporated some heuristic reasoning. The project began on 25-09-2025, and each dataset has since grown by one new observation per week.

**Preprocessing and uses**: I have not transformed the datasets. Because it was generated for a Black-Box challenge, it is not intended to reflect real-world phenomena and should not be used for that purpose.

**Distribution and maintenance**: The datasets will be available on this GitHub page before 31-01-2026. It is free to use but will not be updated or maintained.




