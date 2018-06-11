# sankey
Javascript to build a sankey chart with more than 2 levels, with fine control over colours. 
  
This is an alteration of the standard google sankey template (https://developers.google.com/chart/interactive/docs/gallery/sankey). The google template **does not render** if groups in different levels have the same name, which was a problem for me as I had the same groups in three levels. I overcame this by inserting a space *in front* of all of the labels in the middle layer, and a space *behind* the layers in the third layer. You could add extra levels by adding multiple spaces. These spaces are then removed when the chart is rendered.
  
 To produce your own chart, you need to put your own data in the data.addRows function. If no label is repeated across different levels (you don't have any A -> A type data) you don't need to worry about strategically adding spaces.
 
 To control the colours, add the hex codes after **var colors**. If you have as many lines in var colors as you have links between categories, you will have a different colour for each stream in the chart. Highlight a specific stream by changing its colour! 
 
 Use **var options** to set the size of the chart. 
 
 Remember that you are storing the data in the js, so sharing this code is the same as sharing your data. 
 
 Portions of this code are modifications based on work created and shared by Google and used according to terms described in the Creative Commons 3.0 Attribution License.
