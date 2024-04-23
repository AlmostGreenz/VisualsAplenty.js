# VisualsAplenty.js

Official Site: https://ryanbgreen.ca/visualsaplenty

# Getting Started:

<p>Welcome to the world of VisualsAplenty.js! We'll get you started in a pinch, but
first we have to make sure you're good to go.</p>

<p>Please ensure that you have <a href="https://fontawesome.com/">Font Awesome
    v5.15.4+</a> included in your webpage to make use of VisualsAplenty.js's full functionality.</p>

<p>Now, let's let's walk through how to create instances of the objects that
    VisualsAplenty.js provides.</p>

    
<pre><code>
// in your HTML file, include the tag: &lt;script&gt;defer src="/path/to/VisualsAplenty.js">&lt;/script&gt;

// sample bar graph

// here is a sample array of objects containing the data to be displayed
const tvData = [
{
Show: "LOST",
Count: 145
},
{
Show: "Sherlock",
Count: 99,
}
]

const tvTableDiv = document.querySelector('.tvTableDiv'); // get the parent element you want the graph to be displayed in

// create the BarGraph instance, resulting in the BarGraph to be drawn within the parent element specified
const favTVShow = new BarGraph("Favourite TV Show", tvData, "Count", "Show", tvTableDiv);

//---------------------------------------------------------------------------------------------------------------------------------
// sample scatter plot
const winLoseData = [
{
Name: "Toronto Maple Leafs",
Wins: 50,
Losses: 80
},
{
Name: "Toronto Raptors",
Wins: 30,
Losses: 90
}
]

const numWinLoseDiv = document.querySelector('.numWinLoseDiv');

// create the ScatterPlot instance, resulting in the ScatterPlot to be drawn within the parent element specified
const winLose = new ScatterPlot("Toronto Team 2021 Win Rate", winLoseData, "Wins", "Losses", numWinLoseDiv, 'Name');
winLose.setLegendVisibility(true); // ScatterPlot by default has no legend, but we can enable it

//---------------------------------------------------------------------------------------------------------------------------------
// sample pie chart
const birdWatchData = [
{
Count: 50,
Name: "Sparrow"
},
{
Count: 30,
Name: "Falcon"
}
]

const pieChartDiv = document.querySelector('.pieChartDiv');

// create the PieChart instance, resulting in the PieChart to be drawn within the parent element specified
const pieChartExample = new PieChart("Bird Watching Data 2021", birdWatchData, "Count", "Name", pieChartDiv);
</code></pre>

<p>Now, go out and create!</p>

Documentation: https://ryanbgreen.ca/visualsaplenty/documentation

Examples: https://ryanbgreen.ca/visualsaplenty/examples