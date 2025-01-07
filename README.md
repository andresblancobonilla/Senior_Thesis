# Senior_Thesis
## Code for senior thesis "Racial Artifacts in the COCO Dataset"
### Adapted from Meister and Zhao et al's work on gender artifacts (https://princetonvisualai.github.io/gender-artifacts/) and Wang et al.'s work on bias mitigation (https://github.com/princetonvisualai/DomainBiasMitigation)
My paper, extending previous work on gender bias, investigates racial artifacts in the
Common Objects in Context (COCO) dataset, which are visual cues in the images of
the dataset that are correlated with race and learnable by a machine learning model.
Using recently crowd-sourced Fitzpatrick skin type annotations on the dataset, I train
a racial artifacts model to classify images as lighter(-skinned) or darker(-skinned),
and evaluate its performance after the image is transformed in various ways to remove
or obscure different aspects of it, such as the color of the image or the faces of the
people, to see if the model can still learn some correlation between the skin types.
I quantitatively analyze performance and qualitatively analyze example images for
these experiments to determine what these correlations might be, and discuss find-
ings and implications. I then investigate possible downstream effects of these racial
artifacts by training an object classification model and analyzing how its performance,
and performance disparity between skin types, change after these image transforma-
tions are applied to the model’s input. This work aims to facilitate understanding of
racial bias in visual datasets and guide bias-aware fairness interventions and dataset
construction in the future.
