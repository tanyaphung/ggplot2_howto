# ggplot2_howto
How to plot with ggplot2 in R

### 1. How to reorder x axis

### 2. How to plot density plot for 2 datasets

```
data_1 = read.table(data_1)
data_2 = read.table(data_2)

ggplot() +
  geom_density(aes(x=data_1[,1], color= "Data 1"), size=1) +
  geom_density(aes(x=data_2[,1], color="Data 2"), size=1) +
  scale_color_manual("",
                     breaks = c("Data 1", "Data 2"),
                     values = c("Data 1" = "black", "Data 2" = "blue"))
```
