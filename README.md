🥗 Project 3: Hypothesis Testing on Nutrition and Diet from Scraped data
📌 Overview
This project aims to evaluate general assumptions about the effectiveness of plant-based and animal-based foods for weight loss and muscle gain using statistical hypothesis testing and nutritional data analysis.

We tested two main hypotheses:

People who lose weight should eat plant-based foods.

People who need to gain muscle should eat animal-based foods.

👥 Group Members
Lê Trọng Nghĩa (Team Leader)

Nguyễn Thiên Phúc

Bành Đức Khánh

Lê Viết Tố Khoa

Lê Hoàng Nguyên

🧪 Hypotheses
Hypothesis	Statement
H1	People who lose weight should eat plant-based foods
H2	People who want to gain muscle should eat animal-based foods

🧰 Methodology
🔍 Data Collection
Web scraping of ~2500 recipes from Tasty.com using Parsehub and BeautifulSoup.

Nutritional data fetched using the CalorieNinjas API.

⚙️ Data Features Collected
sugar_g, fiber_g, sodium_mg, potassium_mg, fat_saturated_g,
fat_total_g, cholesterol_mg, protein_g, carbohydrates_total_g.

🧹 Preprocessing
Corrupted or empty links were filtered automatically.

Nutritional values were normalized and manually weighted based on the hypothesis context.

📊 Statistical Testing
Two-sample Z-tests were performed to compare mean suitability scores between plant-based and animal-based foods:

Hypothesis 1 (Weight Loss)

Result: Rejected (T = -10.64, not in rejection region)

Conclusion: Not enough evidence to prove plant-based is better for weight loss.

Hypothesis 2 (Muscle Gain)

Result: Accepted (T = -14.31, in rejection region)

Conclusion: Strong evidence that animal-based food supports muscle gain.

📈 Visualizations
Boxplots and bar graphs were created to visually compare nutrient distributions.

Plots clearly highlighted trends in calorie density, fiber, and protein content between food types.

✅ Key Findings
Plant-based foods: High in fiber, lower in calories.

Animal-based foods: Higher protein, better for muscle growth.

⚠️ Limitations
Limited dataset size and diversity.

External health factors (exercise, sleep, genetics) not controlled.

CalorieNinjas API does not cover vitamins or micronutrients.

📚 References
World Health Organization (WHO)

National Institutes of Health (NIH)

British Journal of Sports Medicine (BJSM)

CalorieNinjas API
