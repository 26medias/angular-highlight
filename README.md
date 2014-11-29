# Angular-Highlight #
Highlight keywords in a text.

Keywords will be wrapped in `<span class="angular-highlight"></span>`. The classname can be changed with the  optional parameter `highlight-class`.

## Demo ##
[Click here to see the demo.](http://26medias.github.io/angular-highlight/ "Demo")

## Installation ##

Load AngularJS and Angular-Highlight:

	<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.2.27/angular.min.js" type="text/javascript"></script>

	<script src="angular-highlight.js" type="text/javascript"></script>

Include the "angular-highlight" dependency in your module:

	var app = angular.module('main', ['angular-highlight']);

Setup the variables

	app.controller('mainCtrl', function ($scope) {
					
		$scope.keywords = "china, bank, asia pacific";
		
		$scope.demoText = 'China cut interest rates unexpectedly on Friday, stepping up a campaign to prop up growth in the world\'s second-largest economy as it heads toward its slowest growth in nearly a quarter century. <br /> The cut-the first such move in over two years-came as factory growth has stalled and the property market, long a pillar of growth, has remained weak, dragging on broader activity and curbing demand for everything from furniture to cement and steel. <br /> "It\'s a surprise, another Friday night special," said Mark Williams, chief Asia economist with Capital Economics in London. "It may not have a major impact on GDP growth-that depends on if policymakers also allow the rate of credit growth to pick up." <br />Read MoreOil nears $80 on China rate cut, possible OPEC move<br /> The People\'s Bank of China said it was cutting one-year benchmark lending rates by 40 basis points to 5.6 percent. It lowered one-year benchmark deposit rates by less-25 basis points. The changes take effect from Saturday. <br />The central bank also took a step to free up deposit rates, allowing banks to pay depositors 1.2 times the benchmark level, up from 1.1 times previously. <br /> "They are cutting rates and liberalising rates at the same time so that the stimulus won\'t be so damaging," said Li Huiyong, an economist at Shenyin and Wanguo Securities. <br /> Bank lending tumbled in October and money supply growth cooled, raising fears of a sharper economic slowdown and prompting calls for more stimulus measures, including cutting interest rates. <br /> But many analysts had expected the central bank to hold off on reducing rates for now, since it has opted instead for measures like fiscal spending while trying to balance the need to reform the economy. <br /> Chinese leaders have also repeatedly stressed they would tolerate somewhat slower growth as long as the jobs market remained resilient, even as they rolled out a series of more modest stimulus measures this year. <br /> The risks faced by China\'s economy are not that scary and the government is confident it can head off the dangers, President Xi Jinping told global business leaders earlier this month, seeking to dispel worries about the world\'s economy. <br /> In a speech to chief executives at the Asia Pacific Economic Cooperation CEO Summit, Xi said even if China\'s economy were to grow 7 percent, that would still rank it at the forefront of the world\'s economies.';
	});

Use the directive on the page:

	<div highlight="demoText" keywords="keywords">

You can also define what classname to use for the highlight

	<div highlight="demoText" keywords="keywords" highlight-class="myCustomStyle">

## Note ##
The text will be displayed without filtering. HTML and Javascript in the text will be executed.

If you intend on using that directive with user-generated content, you will be exposed to security issues unless you filter the text first.


# License: MIT #
Copyright (c) 2014 Julien Loutre, Twenty-Six Medias, Inc

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.