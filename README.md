# Ember Chart

[![Build Status](https://travis-ci.org/aomran/ember-cli-chart.svg)](https://travis-ci.org/aomran/ember-cli-chart)

This Ember CLI addon is a simple wrapper for [ChartJS](http://www.chartjs.org/) (v2.8.0).

### Installation

```
$ ember install ember-cli-chart
```

### Usage

In your handlebars template just do:

```hbs
{{ember-chart type=CHARTTYPE data=CHARTDATA options=CHARTOPTIONS width=CHARTWIDTH height=CHARTHEIGHT plugins=CHARTPLUGINS}}
```

* CHARTTYPE: String; one of the following -- `line`, `bar`, `radar`, `polarArea`, `pie` or `doughnut`.
* CHARTDATA: Array; refer to the ChartJS documentation
* CHARTOPTIONS: Object; refer to the ChartJS documentation. This is optional.
* CHARTWIDTH: Number; pixel width of the canvas element. Only applies if the chart is NOT responsive.
* CHARTHEIGHT: Number; pixel height of the canvas element. Only applies if the chart is NOT responsive.
* CHARTPLUGINS: Array; refer to ChartJS documentaion. This is optional.

#### Example

```
{{ember-chart type='pie' data=model.chartData width=200 height=200}}
```

#### More Resources

* [Screencast on creating bar charts with ember-cli-chart](https://www.emberscreencasts.com/posts/46-bar-charts-with-ember-cli-chart)
