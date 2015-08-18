# dashboards
Open-source dashboard template for Plotly graphs, forked from the excellent [keen.io dashboard templates](http://keen.github.io/dashboards/layouts/).

### Steps to make your own dashboard

1. [Click this link to download the code](https://github.com/plotly/dashboards/raw/master/Plotly%20Sample%20Dashboard.zip)

2. Unzip the file and open index.html in a text editor

3. [Find the lines](https://github.com/plotly/dashboards/blob/master/index.html#L67) with "iframe" and replace the src with the URL of your Plotly graphs. Don't forget to add the ".embed"! 

[More about embedding plotly graphs with iframes](http://help.plot.ly/embed-graphs-in-websites/)

4. Save index.html and double-click to open in your browser - You should see your plotly graphs in the dashboard now.

[Live example](https://plot.ly/python/dashboard/)

![alt text](http://i.imgur.com/51BoA90.gif "Python powered dashboard")

### Advanced: Adding JavaScript controls

You can add JavaScript controls to any Plotly graph iframe.

See examples of adding a moving average, buttons, and click callbacks.

To run postMessage examples locally on your desktop, you have to open index.html with a WebServer:

1. Open your terminal and naviate to the dashboard folder where index.html is.

2. Start SimpleHTTPServer:

```python -m SimpleHTTPServer 8000```

![alt text](http://i.imgur.com/I2hlyLO.png "SimpleHTTPServer")

3. Navigate to [http://localhost:8000/](http://localhost:8000/) in your browser. You should see the dashboard from index.html.

![alt text](http://i.imgur.com/xace7US.gif "Plotly postmessage slider")
