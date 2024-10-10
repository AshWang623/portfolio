| [home page](https://github.com/AshWang623/portfolio/blob/main/README.md) | [visualizing debt](/dataviz2.md) | [critique by design](/MakeoverMonday.md) | [final project I](/final_project_1.md) | [final project II](/final_project_1.md) | [final project III](final_project_part_3) |

# Original data visualization:
https://ourworldindata.org/time-use#who-do-we-spend-time-with-across-our-lifetime

This graph shows the average time Americans spent with different people in their lives, by age.
I chose this chart because it has a wide audience due to its straightforward theme that resonates easily. 
In addition, the data presented in this chart is very detailed and has room for digging in.

Data Visualization Effectiveness Profile insights:

Based on the critique method, my ratings for the graph's usefulness, completeness, and truthfulness are relatively high. The visualization is a comprehensive and accurate demonstration of the dataset. 
The ratings for aesthetics and engagement are neutral. The graph has a clean graph style and readable labels, yet the information density makes it less pleasing and also reduces engagement.
The ratings for perceptibility and intuitiveness are lower. Grasping and interpreting the trends take more effort than desired due to the overlapping lines.
Therefore, I decided to put my focus on simplifying the chart by improving the aesthetics and enhance the clarity of the lines.

# Sketched solution

To make the first draft of the solution in Tableau, I followed some instructions in the Watch Me Viz video(https://www.youtube.com/watch?v=XZliCbAyBX8&t=376s) of this dataset.

<div class='tableauPlaceholder' id='viz1726698209765' style='position: relative'><noscript><a href='#'><img alt='Who Americans spend their time withAverage time spent in minutes per day by the age of the respondent. This is based on averages from surveys spanning 2009 to 2019. ' src='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Bo&#47;Book1_17256444146430&#47;Sheet1&#47;1_rss.png' style='border: none' /></a></noscript><object class='tableauViz'  style='display:none;'><param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> <param name='embed_code_version' value='3' /> <param name='site_root' value='' /><param name='name' value='Book1_17256444146430&#47;Sheet1' /><param name='tabs' value='no' /><param name='toolbar' value='yes' /><param name='static_image' value='https:&#47;&#47;public.tableau.com&#47;static&#47;images&#47;Bo&#47;Book1_17256444146430&#47;Sheet1&#47;1.png' /> <param name='animate_transition' value='yes' /><param name='display_static_image' value='yes' /><param name='display_spinner' value='yes' /><param name='display_overlay' value='yes' /><param name='display_count' value='yes' /><param name='language' value='en-US' /><param name='filter' value='publish=yes' /></object></div>                
<script type='text/javascript'>                    
  var divElement = document.getElementById('viz1726698209765');                    
  var vizElement = divElement.getElementsByTagName('object')[0];                    vizElement.style.width='100%';vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
  var scriptElement = document.createElement('script');                    
  scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    vizElement.parentNode.insertBefore(scriptElement, vizElement);                
</script>

In this draft, I tried to make the original graph simpler and clearer through the following adjustments:

1. Remove dots on the lines

2. Remove labels on the x and y-axis, and add a description of the measurement in the title

3. Use more contrasting colors to distinguish the lines

4. Simplify the category names

Despite being more aesthetically pleasing, the graph's main issues remain unsolved: Several lines intersect and overlap, especially between the ages of 20 and 60, making it difficult to distinguish trends. The information is overwhelming and lack focus with too many categories and data points, making it difficult to grasp the most significant patterns quickly. 

It's difficult to address these issues while maintaining the integrity of the original data. I had assumed some potential improvements, yet they need validation through the viewers' responses:

1. Change to a stacked bar chart to avoid the lines' overlap problem. This would pivot the focus of the visualization from the trend of each category to the ratio among categories, which falls short of the original intention.
   
2. Remove or aggregate certain categories to avoid clutter. Again, this will result in a loss of information, which may not be what the audience wants in exchange for readability.

3. Segment the x-axis into different age groups. This may help guide the audience to focus on one segment at a time to identify and interpret the trends.

# Interview results
I utilized the seed question sets of the in-class critique for the interview. Here is the summarization of responses：

What worked?

The line chart is a good choice in terms of intuitiveness. The viewers are more interested in the trend of each line than their relationships.
The completeness of the original data is favorable for viewers interested in the topic and who would like to spend a longer time parsing. However, for those with limited watch time, it's hard to draw many conclusions despite all the information given. All viewers identify the growing trend of time spent alone at first glance, as it stands out from the cluster.

What didn't work?

The lines are too busy together. It's relatively easier to focus on one line and recognize the pattern, but a lot harder to select two or three lines at a time and compare them, as the other lines would be distracting. Even though it's not the priority, the viewers do try to compare different lines and find correlations, most times between time spent with partner, family, and children.

What questions came up?

To the viewers, there is some ambiguity in the categories. In this dataset, children and partners are excluded from the family category. Further clarification may be needed in the annotation.
The viewers are also curious about the reason behind each dominant pattern and turning points.

# Final solution

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tableau Embed Test</title>
</head>
<body>
    <!-- Tableau Embed Code Start -->
    <div class='tableauPlaceholder' id='viz1726712223515' style='position: relative'>
        <noscript>
            <a href='#'>
                <img alt='Who Americans spend their time withAverage time spent in minutes per day by the age of the respondent. This is based on averages from surveys spanning 2009 to 2019.'
                src='https://public.tableau.com/static/images/Bo/Book2_17267122058590/Sheet14/1_rss.png' style='border: none' />
            </a>
        </noscript>
        <object class='tableauViz'  style='display:none;'>
            <param name='host_url' value='https%3A%2F%2Fpublic.tableau.com%2F' /> 
            <param name='embed_code_version' value='3' /> 
            <param name='site_root' value='' />
            <param name='name' value='Book2_17267122058590/Sheet14' />
            <param name='tabs' value='no' />
            <param name='toolbar' value='yes' />
            <param name='static_image' value='https://public.tableau.com/static/images/Bo/Book2_17267122058590/Sheet14/1.png' />
            <param name='animate_transition' value='yes' />
            <param name='display_static_image' value='yes' />
            <param name='display_spinner' value='yes' />
            <param name='display_overlay' value='yes' />
            <param name='display_count' value='yes' />
            <param name='language' value='en-US' />
            <param name='filter' value='publish=yes' />
        </object>
    </div>                
    <script type='text/javascript'>
        var divElement = document.getElementById('viz1726712223515');                    
        var vizElement = divElement.getElementsByTagName('object')[0];                    
        vizElement.style.width='100%';
        vizElement.style.height=(divElement.offsetWidth*0.75)+'px';                    
        var scriptElement = document.createElement('script');                    
        scriptElement.src = 'https://public.tableau.com/javascripts/api/viz_v1.js';                    
        vizElement.parentNode.insertBefore(scriptElement, vizElement);                
    </script>
    <!-- Tableau Embed Code End -->
</body>
</html>

For the final version, I added an interactive filter that allows the viewers to tick the lines they want to observe and compare individually. I also segmented the x-axis with a few reference lines by the four life stages. The segmentation leads the viewers to notice the correlation between the turning points of the lines and life stage transitions.
