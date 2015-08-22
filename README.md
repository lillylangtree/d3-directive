##d3 Angular Directive


This git repository contain a sample application to show how to
include a d3 directives library into a project and insert it into
a html page

clone the project using 

```$ git clone  https://github.com/lillylangtree/d3-directive.git
...```

###directive usage

the directive is an attribute directive named 

	angulard3-bar-graph

The directive accepts parameters
```	
	datajson="<json file>" 
	xaxis-name = "<x-axis label>" 
	xaxis-pos = "<x-axis label position in pxs" 
	yaxis-name = "<y-axis label>" 
	yaxis-pos = "<y-axis label position in pxs" 
	d3-format= "<d3 format>"  
```	
###Sample Usage
```
<div id="d3bar" angulard3-bar-graph datajson="'sample.json'" 
									xaxis-name = "'Year'" 
									xaxis-pos = "905" 
									yaxis-name = "'Frequency'" 
									yaxis-pos = "6" 
									d3-format= "'.0%'"  >
</div>
```

where 'sample.json' is of the form of an array of json objects
```
[
{"letter":"2000","frequency":".08167"},
{"letter":"2001","frequency":".01492"},
{"letter":"2002","frequency":".02780"},
{"letter":"2003","frequency":".04253"},
{"letter":"2004","frequency":".12702"},
{"letter":"2005","frequency":".02288"},
{"letter":"2006","frequency":".02022"},
{"letter":"2007","frequency":".06094"},
{"letter":"2008","frequency":".06973"},
{"letter":"2009","frequency":".00153"}
]
```