# The Diet Problem
Homework Assignment for MSDS 460 
### Project Objective
The purpose of this repository is to leverage linear programming techniques for optimizing a weekly diet plan. It aims to minimize costs while ensuring that daily nutritional requirements are met, focusing on a selection of five packaged foods. This solution is particularly beneficial for individuals looking to strategically design their diets in a cost-effective manner, without compromising on nutritional value.
### Part I - [Food Documentation](https://github.com/Hantao-Lin/Linear-Programming---The-Diet-Problem/blob/main/Lable%20Image/Diet%20Problem%20Modeling.pdf)
In this problem, we used the following five packaged foods:
- [Spam Luncheon Meat](https://github.com/Hantao-Lin/Linear-Programming---The-Diet-Problem/blob/main/Lable%20Image/Spam%20Luncheon%20Meat.png)
- [Total Whole Grain Cereal](https://github.com/Hantao-Lin/Linear-Programming---The-Diet-Problem/blob/main/Lable%20Image/Total%20Whole%20Grain%20Cereal%20-%2016oz%20-%20General%20Mills.png)
- [Green Giant Vegetable Blend](https://github.com/Hantao-Lin/Linear-Programming---The-Diet-Problem/blob/main/Lable%20Image/Green%20Giant%20Vegetable%20Blend.jpg)
- [Wild Alaskan Pink Salmon](https://github.com/Hantao-Lin/Linear-Programming---The-Diet-Problem/blob/main/Lable%20Image/Wild%20Alaskan%20Pink%20Salmon.jpg)
- [Organic Vanilla Soy Beverage](https://github.com/Hantao-Lin/Linear-Programming---The-Diet-Problem/blob/main/Lable%20Image/Organic%20Vanilla%20Soy%20Beverage.jpg)
### Part II - Linear Programming Problem: Standard Form
#### Decision Variables
Let's define the decision variables representing the number of servings needed for each food item:
- **x<sub>1</sub>** : Number of servings of Spam Luncheon Meat
- **x<sub>2</sub>** : Number of servings of Total Whole Grain Cereal
- **x<sub>3</sub>** : Number of servings of Green Giant Vegetable Blend
- **x<sub>4</sub>** : Number of servings of Wild Alaskan Pink Salmon
- **x<sub>5</sub>** : Number of servings of Organic Vanilla Soy Beverage
#### Objective Function
The goal is to minimize the overall cost of these servings. The cost function, denoted as Z, is given by: 

**Minimize** Z = 0.9x<sub>1</sub> + 0.62x<sub>2</sub> + 0.86x<sub>3</sub> + 1.3x<sub>4</sub> +0.62x<sub>5</sub>
#### Weekly Nutrition Constraint 
The following are the weekly nutritional constraints:
- **Sodium Constriant**: The total servings of all foods should have a sodium content of at most 35000 mg \
 790x<sub>1</sub> + 190<sub>2</sub> + 210x<sub>3</sub> + 260x<sub>4</sub> + 95x<sub>5</sub> &le; 35000
- **Energy Constriant**: The total energy provided by all foods should be at least 14000 calories. \
 180x<sub>1</sub> + 140x<sub>2</sub> + 45x<sub>3</sub> + 100x<sub>4</sub> + 100x<sub>5</sub> &ge; 14000
- **Protein Constriant**:The total protein content should be at least 350 grams. \
 7.41x<sub>1</sub> + 3x<sub>2</sub> + 2x<sub>3</sub> + 17x<sub>4</sub> + 7x<sub>5</sub> &ge; 350
- **Vitamin D Constriant**:The total Vitamin D content should be at least 140 micrograms.\
 0x<sub>1</sub> + 4x<sub>2</sub> + 0x<sub>3</sub> + 15.9x<sub>4</sub> + 5x<sub>5</sub> &ge; 140
- **Calcium Constriant**:The total calcium content should be at least 9100 mg. \
 7.84x<sub>1</sub> + 40x<sub>2</sub> + 22x<sub>3</sub> + 200x<sub>4</sub> + 300x<sub>5</sub> &ge; 9100
- **Iron Constriant**: The total iron content should be at least 126 mg. \
 0.5x<sub>1</sub> + 18x<sub>2</sub> + 1x<sub>3</sub> + 0.4x<sub>4</sub> + 1x<sub>5</sub> &ge; 126
- **Potassium Constriant**: The total potassium content should be at least 32900 mg. \
 128.84x<sub>1</sub> + 150x<sub>2</sub> + 185x<sub>3</sub> + 280x<sub>4</sub> + 280x<sub>5</sub> &ge; 32900
### Part III
- [Python File](https://github.com/Hantao-Lin/Linear-Programming---The-Diet-Problem/blob/main/Code%20and%20Text%20Result/Diet_Problem.ipynb)
- [No Variety Text Result](https://github.com/Hantao-Lin/Linear-Programming---The-Diet-Problem/blob/main/Code%20and%20Text%20Result/No%20Variety%20Result.txt)
- [Consume Each Food at Least Once Text Result](https://github.com/Hantao-Lin/Linear-Programming---The-Diet-Problem/blob/main/Code%20and%20Text%20Result/Each%20Food%20Consume%20at%20Least%20Once.txt)
