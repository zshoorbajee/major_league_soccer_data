<html>
<head>
  <style>
    .error {
        color: red;
    }
  </style>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm//vega@5"></script>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm//vega-lite@4.17.0"></script>
  <script type="text/javascript" src="https://cdn.jsdelivr.net/npm//vega-embed@6"></script>
</head>
<body>
  <div id="vis"></div>
  <script>
    (function(vegaEmbed) {
      var spec = {"config": {"view": {"continuousWidth": 400, "continuousHeight": 300}, "axisX": {"labelFont": "Calibri", "labelFontSize": 12.5, "labelAngle": -60, "titleFont": "Calibri", "titleFontSize": 15}, "axisY": {"labelFont": "Calibri", "labelFontSize": 12.5, "titleFont": "Calibri", "titleFontSize": 15, "format": "$.2s"}, "title": {"font": "Calibri", "fontSize": 20, "anchor": "middle"}}, "data": {"name": "data-7bc46a0df22bcc74bbcbba9ec52533e6"}, "mark": "bar", "encoding": {"color": {"field": "guar_comp_2022", "legend": {"format": "$.2s", "title": "Avg. Guaranteed Compensation"}, "type": "quantitative"}, "tooltip": [{"field": "club", "title": "MLS Team"}, {"field": "guar_comp_2022", "format": "$,.2f", "title": "Avg. guaranteed compensation"}], "x": {"field": "club", "sort": "-y", "title": "Team", "type": "nominal"}, "y": {"field": "guar_comp_2022", "title": "Average guaranteed compensation", "type": "quantitative"}}, "title": "MLS Average Guaranteed Player Compensation by Team", "$schema": "https://vega.github.io/schema/vega-lite/v4.17.0.json", "datasets": {"data-7bc46a0df22bcc74bbcbba9ec52533e6": [{"club": "Toronto FC", "guar_comp_2022": 1111542.3448275863}, {"club": "LA Galaxy", "guar_comp_2022": 853228.5625}, {"club": "Inter Miami", "guar_comp_2022": 733159.9393939395}, {"club": "St. Louis SC", "guar_comp_2022": 716774.8888888889}, {"club": "Chicago Fire", "guar_comp_2022": 667440.1034482758}, {"club": "LAFC", "guar_comp_2022": 612964.1290322581}, {"club": "Seattle Sounders FC", "guar_comp_2022": 606562.3571428572}, {"club": "Atlanta United", "guar_comp_2022": 606252.8918918918}, {"club": "Columbus Crew", "guar_comp_2022": 596426.9333333333}, {"club": "New England Revolution", "guar_comp_2022": 580767.28125}, {"club": "Sporting Kansas City", "guar_comp_2022": 545785.3333333334}, {"club": "Houston Dynamo", "guar_comp_2022": 527108.90625}, {"club": "FC Cincinnati", "guar_comp_2022": 525196.3548387097}, {"club": "New York City FC", "guar_comp_2022": 500125.69696969696}, {"club": "FC Dallas", "guar_comp_2022": 492552.59375}, {"club": "Austin FC", "guar_comp_2022": 487992.86666666664}, {"club": "Nashville SC", "guar_comp_2022": 471526.0}, {"club": "DC United", "guar_comp_2022": 465210.0571428572}, {"club": "Vancouver Whitecaps", "guar_comp_2022": 438151.4411764706}, {"club": "Orlando City SC", "guar_comp_2022": 398533.73333333334}, {"club": "Real Salt Lake", "guar_comp_2022": 394843.1891891892}, {"club": "Portland Timbers", "guar_comp_2022": 392327.7586206897}, {"club": "CF Montreal", "guar_comp_2022": 373119.3142857143}, {"club": "Philadelphia Union", "guar_comp_2022": 370010.25}, {"club": "Charlotte FC", "guar_comp_2022": 364426.90625}, {"club": "San Jose Earthquakes", "guar_comp_2022": 356742.4}, {"club": "Minnesota United", "guar_comp_2022": 338095.63636363635}, {"club": "Colorado Rapids", "guar_comp_2022": 330342.34375}, {"club": "New York Red Bulls", "guar_comp_2022": 311044.70967741933}, {"club": "Major League Soccer", "guar_comp_2022": 173916.66666666666}]}};
      var embedOpt = {"renderer": "svg", "actions": false, "mode": "vega-lite"};

      function showError(el, error){
          el.innerHTML = ('<div class="error" style="color:red;">'
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