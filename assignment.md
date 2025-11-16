# Assignment

## Brief

Write the Python codes for the following questions.

## Instructions

Paste the answer as Python in the answer code section below each question.

### Question 1

Question: How do you create a 2x2 subplot grid in matplotlib and select the first subplot?

Answer:

```python
fig = plt.figure()
ax1 = fig.add_subplot(2, 2, 1)
```

### Question 2

Question: How do you plot a line and set the color to red and style to dash in a matplotlib plot?

```python
x = [1, 2, 3, 4]
y = [1, 4, 9, 16]
```

Answer:

```python
plt.plot(x, y, 'ro--')
```

### Question 3

Question: How do you plot a histogram with 30 bins for `data` in matplotlib?

```python
data = np.random.randn(1000)
```

Answer:

```python
plt.hist(data, bins=30, color="black")
plt.show()
```

### Question 4

Question: How can you set the x-axis and y-axis labels in a matplotlib plot?

Answer:

```python
ax.set_xlabel("Renamed X Axis")
ax.set_ylabel("Renamed Y Axis")
```

### Question 5

Question: How do you create a bar plot in seaborn using the `tips` dataset to show the average tip amount per day?

```python
import seaborn as sns
tips = sns.load_dataset('tips')
```

Answer:

```python
sns.barplot(data=tips, x='tip', y='day')
#By default, sns.barplot() calculates the average tip amount per day.
```

### Question 6

Question: How do you create a box plot for total_bill categorized by day in the `tips` dataset using seaborn?

Answer:

```python
sns.catplot(x='day', y="total_bill", kind="box", data=tips)
#Quite a number of outliers – probably because those outliers were not filtered out, i.e. the entire 'tips' dataset was considered

```

## Submission

- Submit the URL of the GitHub Repository that contains your work to NTU black board.
- Should you reference the work of your classmate(s) or online resources, give them credit by adding either the name of your classmate or URL.
