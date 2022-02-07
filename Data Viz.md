# line plot

# import libraries
- seaborn atumatically installs these libraries 
*matplotlib*
*scipy*
*pandas*
*numpy*



```python
# import libraries 
import seaborn as sns
import matplotlib.pyplot as plt

# load dataset
phool = sns.load_dataset("iris")
phool

# draw a line plot
sns.lineplot(x="sepal_length",y="sepal_width",data=phool)
plt.show()
```

# Adding titles 


```python
# import libraries 
import seaborn as sns
import matplotlib.pyplot as plt

# load dataset
phool = sns.load_dataset("iris")
phool

# draw a line plot
sns.lineplot(x="sepal_length",y="sepal_width",data=phool)
plt.title("Pholo ka plot")
plt.show()
```

# Adding limits 


```python
# import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
# load dataset
phool = sns.load_dataset("iris")
phool

# draw a line plot
sns.lineplot(x="sepal_length",y="sepal_width",data=phool)
plt.title("Pholo ka plot")
plt.xlim(50)
plt.ylim(50)
plt.show()
```

# set styles 
- darkgrid
- whitegrid
- dark 
- white 
- ticks


```python
# import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
# load dataset
phool = sns.load_dataset("iris")
phool

# draw a line plot
sns.lineplot(x="sepal_length",y="sepal_width",data=phool)
plt.title("Pholo ka plot")
sns.set_style("dark")
sns.set_style(style=None,rc=None)
plt.show()
```

# size of figure


```python
# import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
# load dataset
phool = sns.load_dataset("iris")
phool

# draw a line plot
sns.lineplot(x="sepal_length",y="sepal_width",data=phool)
plt.title("Pholo ka plot")
plt.figure(figsize=(8,6))
plt.show()
```

# Bar plot 


```python
# import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
# load dataset
phool = sns.load_dataset("iris")
phool

# draw a line plot
sns.barplot(x="species",y="sepal_width",data=phool)
plt.title("Pholo ka plot")
plt.show()
```

# Horizontal plot 


```python
# import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
# load dataset
phool = sns.load_dataset("iris")
phool

# draw a line plot
sns.barplot(x="sepal_width",y="species",data=phool)
plt.title("Pholo ka plot")
plt.show()
```


```python
 # import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
# load dataset
phool = sns.load_dataset("iris")
phool

# draw a line plot
sns.barplot(x="species",y="petal_length",data=phool)
plt.title("Pholo ka plot")
plt.show()
```


```python
phool
```


```python
 # import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
# load dataset
khasti = sns.load_dataset("titanic")
khasti

# draw a line plot
sns.barplot(x="who",y="alone",hue="sex",data=khasti)
plt.title("khasti ka plot")
plt.show()
```

# reversing order of axies 


```python
 # import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
# load dataset
khasti = sns.load_dataset("titanic")
khasti

# draw a line plot
sns.barplot(x="who",y="alone",hue="sex",data=khasti,order=["chil","man"])
plt.title("khasti ka plot")
plt.show()
```

# coloring plot 


```python
 # import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
# load dataset
khasti = sns.load_dataset("titanic")
khasti

# draw a line plot
sns.barplot(x="who",y="alone",hue="sex",data=khasti,color="salmon")
plt.title("khasti ka plot")
plt.show()
```

# Removing error bars 


```python
 # import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
# load dataset
khasti = sns.load_dataset("titanic")
khasti

# draw a line plot
sns.barplot(x="who",y="alone",hue="sex",data=khasti,color="salmon",ci=None)
plt.title("khasti ka plot")
plt.show()
```

# Using  Palettes 


```python
 # import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
from numpy import mean
# load dataset
khasti = sns.load_dataset("titanic")
khasti

# draw a line plot
sns.barplot(x="who",y="alone",hue="sex",data=khasti,color="salmon",ci=None,palette='Paired')
plt.title("khasti ka plot")
plt.show()|
```

# Using  Palettes 


```python
 # import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
import numpy
from numpy import mean
# load dataset
khasti = sns.load_dataset("titanic")
khasti

# draw a line plot
sns.barplot(x="who",y="fare",hue="sex",data=khasti,color="salmon",ci=None,palette='Paired',estimator=mean)
plt.title("khasti ka plot")
plt.show()
```

# Using saturation


```python
 # import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
import numpy
from numpy import mean
# load dataset
khasti = sns.load_dataset("titanic")
khasti

# draw a line plot
sns.barplot(x="who",y="fare",hue="sex",data=khasti,color="salmon",ci=None,palette='Paired',estimator=mean,saturation=2)
plt.title("khasti ka plot")
plt.show()
```

# facecolor edgecolor errorcolor lineweidth 


```python
# import libraries 
import seaborn as sns
import matplotlib.pyplot as plt
# load dataset
phool = sns.load_dataset("iris")
phool

# draw a line plot
sns.barplot(x="species",y="sepal_width",data=phool,facecolor=(.3,.3,.5,.2),edgecolor="0",linewidth=3,errcolor=".2")
plt.title("Pholo ka plot")
plt.show()
```

# Box plot


```python
# import libraries 
import seaborn
# canvas baloon board
seaborn.set_style("whitegrid")
kashti= seaborn.load_dataset("titanic")
# facecolor=(.3,.3,.5,.2),edgecolor="0",linewidth=3,errcolor=".2"
# draw a box plot
seaborn.boxplot(x="class",y="fare",data=kashti)
plt.title("kashti ka plot")
plt.show()
```


```python
# import libraries 
import seaborn as sns
# canvas baloon board
seaborn.set_style('whitegrid')
tip = sns.load_dataset("tips")
tip
sns.boxplot(x="day",y="tip",saturation=.5,data=tip,color="#86bd2f")
plt.show()
# facecolor=(.3,.3,.5,.2),edgecolor="0",linewidth=3,errcolor=".2"
# draw a box plot
# seaborn.boxplot(x="class",y="fare",data=kashti)
# plt.title("kashti ka plot")
# plt.show()
```


```python
# import libraries 
import seaborn as sns
import pandas as pd
import numpy as np
seaborn.set_style('whitegrid')
tip = sns.load_dataset("tips")
tip.values
```

# ploting with one column


```python

import seaborn as sns
# canvas baloon board
seaborn.set_style('whitegrid')
tip = sns.load_dataset("tips")
sns.boxplot(x=tip["size"])
plt.show()
```

# Importing the required modules :


```python
import seaborn as sns
# canvas baloon board
seaborn.set_style('whitegrid')
tip = sns.load_dataset("tips")
sns.boxplot(x="tip",y="day",hue="smoker",palette="Accent",dodge=True,data=tip,)
plt.show()
```


```python
import seaborn as sns 
import pandas as pd
import numpy as np
kashti= sns.load_dataset("titanic")
kashti.head(5)
```


```python
sns.boxplot(x="survived",y="age",data=kashti)
plt.show()
```


```python
p1=sns.boxplot(x="survived",y="age",showmeans=True ,data=kashti)
plt.show()
```


```python
sns.boxplot(x="survived",y="age",showmeans=True,meanprops={"marker":"+","markersize":"2","markeredgecolor":"red"},data=kashti)
plt.show()
```


```python
#show levels
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
import numpy as np
kashti= sns.load_dataset("titanic")
sns.boxplot(x="survived",y="age",showmeans=True,meanprops={"marker":"+","markersize":"2","markeredgecolor":"red"},data=kashti)
plt.show()
plt.xlabel("How many survived",size=15)
plt.ylabel("Age in years")
plt.title("Box plot of safina",size=12,weight="bold")
plt.show()
```

# facet wrap facet grid


```python
plt.xlabel("How many survived",size=15,,facet_wrap(~align + sex))
plt.ylabel("Age in years")
plt.title("Box plot of safina",size=12,weight="bold")
plt.show()
```


      File "<ipython-input-11-ba343de628e9>", line 1
        plt.xlabel("How many survived",size=15,facet_wrap(~align + sex))
                                               ^
    SyntaxError: positional argument follows keyword argument
    


# 04- other plots


```python
#line plots with multifacet
```


```python
import seaborn as sns
import numpy as np
import matplotlib.pyplot as plt
import pandas as pd 
nukte=sns.load_dataset("dots")
nukte.head()
# # defining a color palette 

palette = sns.color_palette("rocket_r")
#plot line plot 
sns.relplot(data=nukte,x="time",y="firing_rate",hue="coherence",size="choice",col="align",kind="line",size_order=["T1","T2"],palette=palette,height=5,aspect=.75,facet_kwt=dict(squarex=False))
```


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    <ipython-input-2-51192809b1ba> in <module>
          9 palette = sns.color_palette("rocket_r")
         10 #plot line plot
    ---> 11 sns.relplot(data=nukte,x="time",y="firing_rate",hue="coherence",size="choice",col="align",kind="line",size_order=["T1","T2"],palette=palette,height=5,aspect=.75,facet_kwt=dict(squarex=False))
    

    ~\anaconda3\1\lib\site-packages\seaborn\relational.py in relplot(x, y, hue, size, style, data, row, col, col_wrap, row_order, col_order, palette, hue_order, hue_norm, sizes, size_order, size_norm, markers, dashes, style_order, legend, kind, height, aspect, facet_kws, **kwargs)
       1693 
       1694     # Draw the plot
    -> 1695     g.map_dataframe(func, x, y,
       1696                     hue=hue, size=size, style=style,
       1697                     **plot_kws)
    

    ~\anaconda3\1\lib\site-packages\seaborn\axisgrid.py in map_dataframe(self, func, *args, **kwargs)
        826 
        827             # Draw the plot
    --> 828             self._facet_plot(func, ax, args, kwargs)
        829 
        830         # Finalize the annotations and layout
    

    ~\anaconda3\1\lib\site-packages\seaborn\axisgrid.py in _facet_plot(self, func, ax, plot_args, plot_kwargs)
        844 
        845         # Draw the plot
    --> 846         func(*plot_args, **plot_kwargs)
        847 
        848         # Sort out the supporting information
    

    ~\anaconda3\1\lib\site-packages\seaborn\relational.py in lineplot(x, y, hue, size, style, data, palette, hue_order, hue_norm, sizes, size_order, size_norm, dashes, markers, style_order, units, estimator, ci, n_boot, seed, sort, err_style, err_kws, legend, ax, **kwargs)
       1130         ax = plt.gca()
       1131 
    -> 1132     p.plot(ax, kwargs)
       1133     return ax
       1134 
    

    ~\anaconda3\1\lib\site-packages\seaborn\relational.py in plot(self, ax, kws)
        772         # function will advance the axes property cycle.
        773 
    --> 774         scout, = ax.plot([], [], **kws)
        775 
        776         orig_color = kws.pop("color", scout.get_color())
    

    ~\anaconda3\1\lib\site-packages\matplotlib\axes\_axes.py in plot(self, scalex, scaley, data, *args, **kwargs)
       1645         """
       1646         kwargs = cbook.normalize_kwargs(kwargs, mlines.Line2D)
    -> 1647         lines = [*self._get_lines(*args, data=data, **kwargs)]
       1648         for line in lines:
       1649             self.add_line(line)
    

    ~\anaconda3\1\lib\site-packages\matplotlib\axes\_base.py in __call__(self, *args, **kwargs)
        214                 this += args[0],
        215                 args = args[1:]
    --> 216             yield from self._plot_args(this, kwargs)
        217 
        218     def get_next_color(self):
    

    ~\anaconda3\1\lib\site-packages\matplotlib\axes\_base.py in _plot_args(self, tup, kwargs)
        361                 "2.2", message="cycling among columns of inputs with "
        362                 "non-matching shapes is deprecated.")
    --> 363         return [func(x[:, j % ncx], y[:, j % ncy], kw, kwargs)
        364                 for j in range(max(ncx, ncy))]
        365 
    

    ~\anaconda3\1\lib\site-packages\matplotlib\axes\_base.py in <listcomp>(.0)
        361                 "2.2", message="cycling among columns of inputs with "
        362                 "non-matching shapes is deprecated.")
    --> 363         return [func(x[:, j % ncx], y[:, j % ncy], kw, kwargs)
        364                 for j in range(max(ncx, ncy))]
        365 
    

    ~\anaconda3\1\lib\site-packages\matplotlib\axes\_base.py in _makeline(self, x, y, kw, kwargs)
        253         default_dict = self._getdefaults(set(), kw)
        254         self._setdefaults(default_dict, kw)
    --> 255         seg = mlines.Line2D(x, y, **kw)
        256         return seg
        257 
    

    ~\anaconda3\1\lib\site-packages\matplotlib\lines.py in __init__(self, xdata, ydata, linewidth, linestyle, color, marker, markersize, markeredgewidth, markeredgecolor, markerfacecolor, markerfacecoloralt, fillstyle, antialiased, dash_capstyle, solid_capstyle, dash_joinstyle, solid_joinstyle, pickradius, drawstyle, markevery, **kwargs)
        398         # update kwargs before updating data to give the caller a
        399         # chance to init axes (and hence unit support)
    --> 400         self.update(kwargs)
        401         self.pickradius = pickradius
        402         self.ind_offset = 0
    

    ~\anaconda3\1\lib\site-packages\matplotlib\artist.py in update(self, props)
       1004 
       1005         with cbook._setattr_cm(self, eventson=False):
    -> 1006             ret = [_update_property(self, k, v) for k, v in props.items()]
       1007 
       1008         if len(ret):
    

    ~\anaconda3\1\lib\site-packages\matplotlib\artist.py in <listcomp>(.0)
       1004 
       1005         with cbook._setattr_cm(self, eventson=False):
    -> 1006             ret = [_update_property(self, k, v) for k, v in props.items()]
       1007 
       1008         if len(ret):
    

    ~\anaconda3\1\lib\site-packages\matplotlib\artist.py in _update_property(self, k, v)
        999                 func = getattr(self, 'set_' + k, None)
       1000                 if not callable(func):
    -> 1001                     raise AttributeError('{!r} object has no property {!r}'
       1002                                          .format(type(self).__name__, k))
       1003                 return func(v)
    

    AttributeError: 'Line2D' object has no property 'facet_kwt'



![png](output_49_1.png)


# penguin plot


```python
import seaborn as sns
sns.set_style(style="ticks")
df=sns.load_dataset("penguins")
sns.pairplot(df,hue="species")
```




    <seaborn.axisgrid.PairGrid at 0xb16aac0>




![png](output_51_1.png)



```python
import seaborn as sns
sns.set_style(style="white")

df = sns.load_dataset("penguins")

g = sns.JointGrid(data=df, x="body_mass_g", y="bill_depth_mm", space=0)
g.plot_joint(sns.kdeplot,
             fill=True, clip=((2200, 6800), (10, 25)),
             thresh=0, levels=100, cmap="rocket")
# g.plot_marginals(sns.histplot, color="#03051A", alpha=1, bins=25)
```




    <seaborn.axisgrid.JointGrid at 0xc3662b0>




![png](output_52_1.png)



```python
pip install plotly
```

    Note: you may need to restart the kernel to use updated packages.
    

    WARNING: Retrying (Retry(total=4, connect=None, read=None, redirect=None, status=None)) after connection broken by 'NewConnectionError('<pip._vendor.urllib3.connection.VerifiedHTTPSConnection object at 0x0000000004957430>: Failed to establish a new connection: [Errno 11004] getaddrinfo failed')': /simple/plotly/
    WARNING: Retrying (Retry(total=3, connect=None, read=None, redirect=None, status=None)) after connection broken by 'NewConnectionError('<pip._vendor.urllib3.connection.VerifiedHTTPSConnection object at 0x0000000004957130>: Failed to establish a new connection: [Errno 11004] getaddrinfo failed')': /simple/plotly/
    WARNING: Retrying (Retry(total=2, connect=None, read=None, redirect=None, status=None)) after connection broken by 'NewConnectionError('<pip._vendor.urllib3.connection.VerifiedHTTPSConnection object at 0x00000000049515E0>: Failed to establish a new connection: [Errno 11004] getaddrinfo failed')': /simple/plotly/
    WARNING: Retrying (Retry(total=1, connect=None, read=None, redirect=None, status=None)) after connection broken by 'NewConnectionError('<pip._vendor.urllib3.connection.VerifiedHTTPSConnection object at 0x0000000004951EB0>: Failed to establish a new connection: [Errno 11004] getaddrinfo failed')': /simple/plotly/
    WARNING: Retrying (Retry(total=0, connect=None, read=None, redirect=None, status=None)) after connection broken by 'NewConnectionError('<pip._vendor.urllib3.connection.VerifiedHTTPSConnection object at 0x0000000004951D60>: Failed to establish a new connection: [Errno 11004] getaddrinfo failed')': /simple/plotly/
    ERROR: Could not find a version that satisfies the requirement plotly (from versions: none)
    ERROR: No matching distribution found for plotly
    
