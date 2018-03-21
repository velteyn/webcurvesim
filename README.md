# webcurvesim
<h1>Stock Market Simulator with FIX gateway support</h1>



<p >A generic equity/derivative stock exchange simulator</p>
<p>If you work in financial industry especially in Equity/Derivative trading area, often you wish to have a stock exchange simulator for your application testing. There are a few reasons for this:</p>

<ul>
<li>The test exchange gateways provided by exchange may not be always available. e.g. some are not available after working hours or in weekend.</li>
<li>The test exchange gateways provided by exchange are shared by other brokers and your testing may be interfered by other people.</li>
<li>An exchange simulator provides you the freedom of total controlling when and how to use it since you own the simulator.</li>
<li>You could perform load testing on your application against the simulator where its usually prohibited on the test exchange since it might overload the system and affect testers from other brokers.</li>
<li>It's extreme useful for algorithmic trading testing due to

<ol><li>"you own the market" such that you could generate any scenario for your testing</li>
<li>you can replay the market data for your back testing and even play different strategies or same strategy with different parameters against replay market to fine tune strategy performance.</li></ol></li>
</ul>

<p>Features:</p>

<p>WebCurve simulator provides the following features for you with an open source license(its basically free, please read the license for details):</p>

<ul>
<li>A set of core functions to simulate the exchange behavior.</li>
<li>A FIX gateway supported by QuickFIX/J for your FIX application testing</li>
<li>Market making simulation to provide a simulated market</li>
<li>Market replay function to support replay live market data</li>
</ul>

              
<p>There are 4 sample programs come with this bundle which demonstrate how WebCurve simulator works.</p>
<p>Original author is Dennis Chen, you can contact him here at dennis_d_chen@yahoo.com.</p>
