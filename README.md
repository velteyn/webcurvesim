# webcurvesim
<h1>Stock Market Simulator with FIX gateway support</h1>


If you work for financial industry especially in Equity/Derivative trading area, often you may want a stock exchange simulator for your application testing. There are a few reasons for this:

The test exchange gateways provided by exchange may not be always available. e.g. some are not available after working hours or in the weekend.
The test exchange gateways provided by exchange are shared by other brokers and your testing may be interfered by other people.
An exchange simulator provides you the freedom of total controling when and how to use it since you own the simulator.
You could perform load testing on your application against the simulator where its usually prohibited on the test exchange since it might overload the system and affect testers from other brokers.
It's extreme useful for algorithmic trading testing due to

"you own the market" such that you could generate any scenario for your testing
you can replay the market data for your back testing and even play different strategies or same strategy with different parameters against the replay market to fine tune performance.


<b>Features</b>
<p>
WebCurve simulator provides the following features for you with an open sourcelicense(its basically free, please read the license for details
</p>
A set of core functions to simulate the exchange behavior.
A FIX gateway supported by QuickFIX/J for your FIX application testing
Market making simulation to provide a simulated market
Market replay function to support replay live market data

Known limitation

No stock, price, price step, lot size validation. This would require a huge database implementation.
Only support FIX 4.2. I am happy to implement other versions in a later stage if there are enough interest out there.
Webecurvesim.jar provides a generic interface to java 6/5/1/1.4.2. The sample programs main()s are written and compiled with java 5 so you need to get java 5/6 runtime to play. If your application is at 1.4.x, you are stillable to the webcurvesim.jar lib but just need to write your interface program in 1.4.x way.


There are 4 sample programs come with this bundle which demonstrate how WebCurve simulator works.
Original author is Dennis Chen, you can contact him here at dennis_d_chen@yahoo.com.
