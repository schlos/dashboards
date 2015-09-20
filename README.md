# Plotly dashboards

Open-source dashboard template for plotly graphs, forked from the [keen.io dashboard templates](http://keen.github.io/dashboards/layouts/).


### Make your own dashboard

1. [Download the code](https://github.com/plotly/dashboards/raw/master/Plotly%20Sample%20Dashboard.zip)

2. Unzip the file and open index.html in a text editor

3. [Find the lines](https://github.com/plotly/dashboards/blob/master/index.html#L67) containing the text "iframe" and replace the URL with your plotly graph URL. Don't forget to add the ".embed" ([More about embedding plotly graphs with iframes](http://help.plot.ly/embed-graphs-in-websites/))

4. Save index.html and double-click to open it in your browser.


[Live example](https://plot.ly/python/dashboard/)

![alt text](http://i.imgur.com/51BoA90.gif "Python powered dashboard")

---

### Advanced: Adding JavaScript controls


You can add JavaScript controls to any Plotly graph iframe with [plotly's postMessage API](https://github.com/plotly/postMessage-API).

See examples of adding a [moving average](https://plot.ly/python/range-slider/), [custom buttons](https://plot.ly/python/custom-buttons/), and [zoom callbacks](https://plot.ly/python/zoom-events/).

To run postMessage examples locally on your desktop, you have to open index.html with a WebServer:

![alt text](http://i.imgur.com/I2hlyLO.png "SimpleHTTPServer")


1. Open your terminal and navigate to the dashboard folder where index.html is.

2. Start SimpleHTTPServer ```python -m SimpleHTTPServer 8000```

3. Navigate to [http://localhost:8000/](http://localhost:8000/) in your browser. You should see the dashboard from index.html.

---

### Double slider JavaScript control


![alt text](http://i.imgur.com/xace7US.gif "Plotly postmessage slider")
