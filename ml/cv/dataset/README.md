# Dataset

For the image recognition feature, I narrowed down the scope into Food categorization, and the below link contains a dataset for categorizing food image into 11 different categories such as Bread, Dairy product, Dessert, Egg, Fried food, Meat, Noodles-Pasta, Rice, Seafood, Soup, Vegetable-Fruit. 16643 food images grouped in 11 major food categories. There are 3 splits in this dataset - evaluation, training, and validation.

I have downloaded the data and stored it on AWS S3 bucket with the following structure:

food-image-dataset/
        - evaluation
                - Bread/
                - Dairy product/
                - Dessert/
                - Egg/
                - Fried food/
                - Meat/
                - Noodles-Pasta/
                - Rice/
                - Seafood/
                - Soup/
                - Vegetable-Fruit/
        - training
                - Bread/
                - Dairy product/
                - Dessert/
                - Egg/
                - Fried food/
                - Meat/
                - Noodles-Pasta/
                - Rice/
                - Seafood/
                - Soup/
                - Vegetable-Fruit/
        - validation
                - Bread/
                - Dairy product/
                - Dessert/
                - Egg/
                - Fried food/
                - Meat/
                - Noodles-Pasta/
                - Rice/
                - Seafood/
                - Soup/
                - Vegetable-Fruit/

Original Source Link: https://www.epfl.ch/labs/mmspg/downloads/food-image-datasets/