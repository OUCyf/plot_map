# 更新 Update
## 2020.3.22
绘图过程增加了timeout为6s，尝试次数10次，妈妈再也不用担心plot_map画图卡很久
add 6s timeout and maximun try 10 times

# plot_map

plot_map是一个基于matplotlib的工具，在用geopandas或者pyplot绘制地理图形的时候，你可以用plot_map来添加地图底图  
When you want to plot geo object using python geopandas or matplotlib.pyplot, you can use this module to generate map backgroud.  

只需要用以下代码：  
Just use the following code:  

    plot_map(plt,bounds,zoom = 9,style = 1)

你可以通过改变参数"style"和"styleid"来改变底图的风格样式  
You can change your map style by changing the "style" and "styleid" in the function plot_map  

	bounds -- Set your plotting boundary [lon1,lat1,lon2,lat2] (wgs1984)  
	zoom -- The zoom level of the map  
	style -- From 1 to 7 represent different map styles,1-6 is from openstreetmap and 7 is the mapbox    
	styleid -- if style is set as 7(from mapbox), you can change the styleid here, "dark" or "light" or your own style  

可以实现的效果：  
example：  
<img height="600" src="img/example.png">

更多信息请看：  
see more on the ipynb: Tutorial(https://github.com/ni1o1/plot_map/blob/master/tutorial/Tutorial_of_plot_map.ipynb)
