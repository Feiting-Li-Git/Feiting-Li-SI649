# Feiting-Li-SI649
![image](https://github.com/user-attachments/assets/ffe6098d-d969-4653-a94e-e576bc1e0138)


![image](https://github.com/user-attachments/assets/ce553b5f-d3a3-4747-931c-6300664f947c)

<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <style>
    #vis.vega-embed {
      width: 100%;
      display: flex;
    }

    #vis.vega-embed details,
    #vis.vega-embed details summary {
      position: relative;
    }
  </style>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/vega@5"></script>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/vega-lite@5.20.1"></script>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm/vega-embed@6"></script>
</head>
<body>
  <a href="https://scmcqueen.github.io/si649_hw/reviews_by_char.csv" target="_blank">Download Data</a>
  <div id="vis"></div>
  <script>
    (function(vegaEmbed) {
      var spec = {"config": {"title": {"anchor": "start", "fontSize": 25, "font": "Inter", "color": "#000000"}, "axis": {"titleFontSize": 16, "labelFontSize": 14, "titleFont": "Lato", "labelFont": "Lato", "domain": false, "grid": true, "tickColor": "transparent", "gridColor": "lightgray"}, "legend": {"titleFontSize": 14, "labelFontSize": 12, "titleFont": "Lato", "labelFont": "Lato"}, "background": "white", "view": {"stroke": "transparent"}, "range": {"category": ["#003C96", "#11A69C", "#924AF7", "#D17711", "#0081FE", "#FF5383"], "ordinal": ["#00AB55", "#400387", "#F2681F", "#005062", "#DE2C62", "#660E00"], "diverging": ["#008753", "#005F3E", "#ED0000", "#CC0000", "#6BEC8C", "#F47171", "#FFC58F"]}, "axisX": {"grid": false}, "axisY": {"titleFontSize": 14, "titlePadding": 10}}, "data": {"name": "data-16fdf8762ce31301fd3b52b54a8d2346"}, "mark": {"type": "circle", "size": 30}, "encoding": {"color": {"field": "normalized_percentage", "scale": {"domain": [0, 1], "range": ["#00AB55", "#400387", "#F2681F", "#005062", "#DE2C62", "#660E00"]}, "title": "Percent", "type": "quantitative"}, "tooltip": [{"field": "character", "type": "nominal"}, {"field": "total", "type": "quantitative"}, {"field": "normalized_percentage", "type": "quantitative"}], "x": {"field": "total", "scale": {"domain": [800, 850]}, "title": "Number of Ratings", "type": "quantitative"}, "y": {"field": "normalized_percentage", "scale": {"domain": [0, 1]}, "title": null, "type": "quantitative"}}, "title": {"text": "Favorable Ratings by Number of Ratings", "anchor": "start", "subtitle": "Percent of Favorable Ratings"}, "$schema": "https://vega.github.io/schema/vega-lite/v5.20.1.json", "datasets": {"data-16fdf8762ce31301fd3b52b54a8d2346": [{"character": "Anakin Skywalker", "rating_category": "Favorable", "count": 514, "total": 823, "percentage": 62.454434993924664, "normalized_percentage": 0.6245443499392467}, {"character": "Boba Fett", "rating_category": "Favorable", "count": 291, "total": 812, "percentage": 35.83743842364532, "normalized_percentage": 0.3583743842364532}, {"character": "C-3P0", "rating_category": "Favorable", "count": 703, "total": 827, "percentage": 85.00604594921403, "normalized_percentage": 0.8500604594921403}, {"character": "Darth Vader", "rating_category": "Favorable", "count": 481, "total": 826, "percentage": 58.23244552058111, "normalized_percentage": 0.5823244552058111}, {"character": "Emperor Palpatine", "rating_category": "Favorable", "count": 253, "total": 814, "percentage": 31.08108108108108, "normalized_percentage": 0.3108108108108108}, {"character": "Han Solo", "rating_category": "Favorable", "count": 761, "total": 829, "percentage": 91.79734620024126, "normalized_percentage": 0.9179734620024127}, {"character": "Jar Jar Binks", "rating_category": "Favorable", "count": 242, "total": 821, "percentage": 29.476248477466505, "normalized_percentage": 0.29476248477466505}, {"character": "Lando Calrissian", "rating_category": "Favorable", "count": 365, "total": 820, "percentage": 44.51219512195122, "normalized_percentage": 0.4451219512195122}, {"character": "Luke Skywalker", "rating_category": "Favorable", "count": 771, "total": 831, "percentage": 92.7797833935018, "normalized_percentage": 0.927797833935018}, {"character": "Obi Wan Kenobi", "rating_category": "Favorable", "count": 750, "total": 825, "percentage": 90.9090909090909, "normalized_percentage": 0.9090909090909091}, {"character": "Padme Amidala", "rating_category": "Favorable", "count": 351, "total": 814, "percentage": 43.12039312039312, "normalized_percentage": 0.4312039312039312}, {"character": "Princess Leia Organa", "rating_category": "Favorable", "count": 757, "total": 831, "percentage": 91.0950661853189, "normalized_percentage": 0.910950661853189}, {"character": "R2 D2", "rating_category": "Favorable", "count": 747, "total": 830, "percentage": 90.0, "normalized_percentage": 0.9}, {"character": "Yoda", "rating_category": "Favorable", "count": 749, "total": 826, "percentage": 90.67796610169492, "normalized_percentage": 0.9067796610169492}]}};
      var embedOpt = {"mode": "vega-lite"};

      function showError(el, error){
          el.innerHTML = ('<div style="color:red;">'
                          + '<p>JavaScript Error: ' + error.message + '</p>'
                          + "<p>This usually means there's a typo in your chart specification. "
                          + "See the javascript console for the full traceback.</p>"
                          + '</div>');
          throw error;
      }
      const el = document.getElementById('vis');
      vegaEmbed("#vis", spec, embedOpt)
        .catch(error => showError(el, error));
    })(vegaEmbed);

  </script>
</body>
</html>
