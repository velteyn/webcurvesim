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

<ul><li>A set of core functions to simulate the exchange behavior.</li><li>A FIX gateway supported by QuickFIX/J for your FIX application testing</li><li>Market making simulation to provide a simulated market</li><li>Market replay function to support replay&nbsp;live market data</li></ul>Known limitation<br><ul><li>No stock, price, price step, lot size validation. This would require a huge database implementation.</li><li>Only support FIX 4.2. I am happy to implement other versions in a later stage if &nbsp;there are enough interest out there.</li><li>Webecurvesim.jar
provides generic interface to java 6/5/1/1.4.2. The sample
programs main()s are written and compiled with java 5 so you need to
get java 5/6
runtime to play. If your application is&nbsp;at 1.4.x, you are still
able to the webcurvesim.jar lib but just need to write your interface
program in 1.4.x way.</li></ul><br>There
are 4 sample programs come with this bundle which demonstrate how
WebCurve simulator work. Feel free to contact me at
dennis_d_chen@yahoo.com if you have any questions or want to see any
features to add. <br><br><h2>Samples Programs</h2>Please
unzip&nbsp;webcurvesim.zip to a directory. You can find 4 windows batch
files test1.bat, test2.bat, exchange.bat and trade.bat. Unix users
should find it simple to convert them into shell scripts.<br><br><h3>Test1</h3>This demonstrates how to use the core Exchange class and &nbsp;OrderBook class in a basic way.<br><br><h3>Test2</h3>This&nbsp;demonstrates&nbsp; how to get order and trade updates a call back way.<br><br><h3>Exchange</h3>This demonstrates the exchange simulator in a GUI application with the following features<br><ul><li>Order transaction in interative way</li><li>Market activity simulation</li><li>Market replay</li><li>Serves as a FIX gateway server(see next)</li></ul><br><h3>Trade</h3>This
demonstrates how a simple OMS system interacts with exchange simulator
through FIX 4.2 protocol. This requres the above sample program running
as server.<br><span style="text-decoration: underline; font-weight: bold;">Usage</span><br><ul><li>Create client orders(parent order) with "Enter Order" button.</li><li>Select one or many client orders then send child orders with "Split Order" button.</li><li>Amend client order or child order with "Amend Order" button. Only allow amend down quantity and amend price.</li><li>Cancel client order or child order with "Cancel Order" button.</li></ul><span style="font-weight: bold; text-decoration: underline;">Known issues</span><br><ul><li>No quantity check between parent orders and child orders. It is possible to overfill order.</li><li>Some time you may hit some GUI refresh problems when expanding the order tree.</li></ul><br><h2>Dependent Packages</h2><ul><li>QuickFIX/J</li><li>Appache MINA required by &nbsp;QuickFIX</li><li>SF4J<br></li></ul>

            

<p>Original author is Dennis Chen, you can contact him here at dennis_d_chen@yahoo.com.</p>
