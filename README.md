
# PFAI_projectR

## 📌 Overview
This repository contains assignments and projects related to **R programming** and **RStudio**. It includes exercises on exploring RStudio, practicing built-in functions, working with library packages, and performing advanced data analysis.

---

## 🖥️ Exploring RStudio
This section covers the basics of RStudio and how to navigate its interface.  

- Understanding the **Source, Console, Environment, and other panes** in RStudio.  
- Creating and saving a new R script.  
- Executing individual lines and entire scripts.  
- Viewing the built-in `mtcars` dataset using functions like `str()` and `summary()`.  
- Setting and verifying the **working directory** in RStudio using:  
  ```r
  setwd("your/path/here")
  getwd()
  ```

---

## 🛠 Practicing Built-in Functions
Basic R operations using built-in functions:

- **Descriptive statistics**:  
  ```r
  data <- c(1, 2, 3, 4, 5)
  mean(data)
  median(data)
  # Mode function in R requires a workaround
  ```
- **Sum of even numbers (1 to 100)**:  
  ```r
  sum(seq(2, 100, by = 2))
  ```
- **String concatenation using `paste()`**:  
  ```r
  paste("Hello", "World", sep = " ")
  ```
- **Matrix operations**:  
  ```r
  mat <- matrix(1:9, nrow = 3)
  t(mat)  # Transpose
  det(mat)  # Determinant
  ```

---

## 📦 Working with Library Packages
Using essential R packages for data manipulation and visualization.

1. **Install and use `ggplot2` for scatterplots**:  
   ```r
   install.packages("ggplot2")
   library(ggplot2)
   ggplot(mtcars, aes(x = mpg, y = hp)) + geom_point()
   ```
2. **Filtering data with `dplyr`**:  
   ```r
   install.packages("dplyr")
   library(dplyr)
   iris %>% filter(Species == "setosa") %>% arrange(Sepal.Length)
   ```
3. **Reshaping data using `tidyr`**:  
   ```r
   install.packages("tidyr")
   library(tidyr)
   pivot_longer(iris, cols = starts_with("Sepal"), names_to = "Measurement", values_to = "Value")
   ```
4. **Exploring `data.table` for fast data handling**:  
   ```r
   install.packages("data.table")
   library(data.table)
   dt <- data.table(x = 1:5, y = 6:10)
   dt[, sum(y)]
   ```

---

## 🔬 Advanced Tasks
Using more specialized R packages.

- **Parsing dates using `lubridate`**:  
  ```r
  install.packages("lubridate")
  library(lubridate)
  ymd("2025-03-18")
  ```
- **Scraping web data with `rvest`**:  
  ```r
  install.packages("rvest")
  library(rvest)
  ```
- **Machine learning with `caret`**:  
  ```r
  install.packages("caret")
  library(caret)
  ```
- **Time-series visualization using `xts` and `zoo`**.  

---

## 🎯 Bonus Tasks
- Creating an **R Markdown** report and knitting it into HTML or PDF.  
- Interactive plotting with **`plotly`**.  
- Debugging R scripts and fixing syntax errors.  



---

## group members
-Aena Habib 
-Dua Kamal  https://github.com/D940919

## 📄 License
This project is licensed under the **MIT License**
