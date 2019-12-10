# Project Title
CanadaImmigration

This project analysis some data sets to figure out the reasons to migrate to Canada.

# Prerequisites
Python, Pandas (Jupiter Notebook), Matplotlib

# coding style tests
fig = plt.figure(figsize=(12, 7))
ax = fig.add_subplot(111)
i=0
for i in range(len(graphdata)):
    ax.bar(x+w*i,graphdata[i],w-.015,label=labels[i])

ax.autoscale(tight=True)


plt.legend(loc=(0.2,-.35),ncol=3,fancybox=True,shadow=True,columnspacing=5,labelspacing=.7,fontsize=13)
plt.xticks(x+w*i/2,np.array(data.iloc[:,1:].keys()))
plt.tight_layout()
plt.ylim(0,3000000)
plt.title("Age Histogram")
plt.ylabel("Population")
plt.xlabel("Years\nAge Group")
plt.savefig('agegroup.png')

plt.grid(axis='y',linestyle='--')
plt.show()


