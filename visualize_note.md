## hướng dẫn matplotlib và seaborn 

https://qiita.com/tsuruokax/items/90167693f142ebb55a7d <br>
https://qiita.com/skotaro/items/08dc0b8c5704c94eafb9 <br>
https://qiita.com/skotaro/items/7fee4dd35c6d42e0ebae<br>
https://towardsdatascience.com/all-your-matplotlib-questions-answered-420dd95cb4ff


## example
<code>

fig = plt.figure(figsize=(15,10)) #width * height
sns.set(color_codes=True)

cols = 3 #number of graph in a row (cols)
rows = 6/3 #number of total graph / cols = number of rows

ax = fig.add_subplot(2,3,1) #number of graph in a col, number of graph in a row, index
ax.set_title("CTR")
sns.distplot(df["ctr"], axlabel='ctr')

ax = fig.add_subplot(2,3,2)
ax.set_title("device")
sns.distplot(df["device"], kde=False, bins=20, rug=True, axlabel="device")

ax = fig.add_subplot(2,3,3)
ax.set_title("sex")
sns.distplot(df["sex"], kde=False, bins=20, rug=True, axlabel='sex')

ax = fig.add_subplot(2,3,4)
ax.set_title("age")
sns.distplot(df["age"], kde=False, bins=20, rug=True, axlabel='age')

ax = fig.add_subplot(2,3,5)
ax.set_title("image_size")
sns.distplot(df["image_size"], kde=False, bins=20, rug=True, axlabel='image_size')

ax = fig.add_subplot(2,3,6)
ax.set_title("industry")
sns.distplot(df["industry"], kde=False, bins=20, rug=True, axlabel='industry')

</code>
