# CBSD

Psychologists often use a questionnaire to understand people's behavior based on their responses. Then, the result can be used in many ways, several examples being :
To determine the degree of someone's fitness in a job environment,
To determine if a person is ready or not before adopting a child,
To determine if someone has a specific type of mental disorder,
To determine if someone is a victim of an accident.

However, as these questionnaires' popularity rises, people are becoming more conscious about the relation between their answers and their consequences. Thus, some people fake their answers to get away with the "best" consequences. There are two types of faking answers:

Faking good: Behavior in which subjects present themselves in a favorable manner, endorsing desirable traits and rejecting undesirable ones. In example 1, people lie in the job fitness questionnaire so the employer thinks they are a better person, increasing their job acceptance probability.

Faking bad: Behavior in which subjects present themselves in a less favorable manner, endorsing less desirable traits and rejecting desirable ones.

In example 3, people lie in the mental disorder questionnaire to receive certain health benefits.

Therefore, a system should distinguish whether a response to these questionnaires is honest or dishonest. This problem is a classic binary classification problem from a machine-learning perspective. Traditional machine learning algorithms, such as logistic regression, can be trained to distinguish whether someone is lying with decent accuracy. However, a new problem arose. Every questioner has its own property and a different tendency to fake good or bad. Hence, different machine-learning models had to be used each time. This makes psychologist question the reliability of the model proposed. The ideal method should be replicable across different types of datasets. A research study (or, in this project, a machine learning model) is considered replicable when the entire research process is conducted again, using the same methods but new data, and still yields the same results. This shows that the results of the original study are reliable.

In this project, was attempted to find and propose a replicable machine learning model to distinguish whether a questionnaire response is honest or dishonest. The model will be tested against 16 different datasets, 8 faking good and 8 faking bad. And explored three different avenues for the problems:

Machine learning algorithm paired with model-dependent feature selection ( SelectFromModel() and Forward Selection)
Model-independent feature selection (Chi-Square, Mutual Information)
Machine learning algorithm paired with agnostic feature selection (Permutation Importance)
Machine learning algorithm paired with dimensionality reduction techniques (Principal Component Analysis [PCA], Sparse [PCA] )
5 different machine learning algorithms used for the first and third avenues are: Logistic Regression, Random Forest, SVM, and KNN.

A method that produces high and stable accuracy across datasets will be considered as the replicable method.
