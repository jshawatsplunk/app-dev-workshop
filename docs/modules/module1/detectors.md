## Lab Summary
* Create a Detector from one of you charts

---

### 1. Create a Detector from one of your charts
Logon to your account in SignalFx, and click on DASHBOARDS in the menu.

In **DASHBOARDS** click on your dashboard group (the one with your email address) and then on the dashboard name where the chart you created in the previous lab resides.

OR 

Search for your previously created dashboard's name, and click on that dashboard's name in the results.

![](../images/M1-l2-1.png)
 
Once you see the chart...
Click on the bell icon  on your chart and on New Detector From Chart - ADD YOUR INITIALS TO THE NAME (see next step).
We are going to create a new alert detector from the chart.

![](../images/M1-l2-2.png) 

IMPORTANT - In the window that opens, add your initials in front of the proposed text, and click on Create Alert Rule.
It should be something like this: LI's Latency Chart Detector.

![](../images/M1-l2-3.png)  

In the detector window, inside Alert signal, the signal we will alert on is marked with a bell.
The bell in the 'Alert on' column indicates which Signal is being used to generate the alert.

![](../images/M1-l2-4.png)  

Click on Proceed to Alert Condition.
On Alert Condition, click on Static Threshold and then on Proceed to Alert Settings.

![](../images/M1-l2-5.png)  

In Alert Settings, enter the value "290" in the Threshold box and change Time on top right to past day.

![](../images/M1-l2-6.png)   

Once you set an alert condition, SignalFx shows how many alerts you would get based on the current settings, and in the timeframe set on the upper right corner - in this case, the past day.
Immediately, the platform will start analysing the signals with the current settings, and perform something we call a Pre-flight Check, This enables me to test the alert conditions using the historical data in the platform, to ensure the settings are logical and will not inadvertently generate an alert storm, removing the guess work from configuring alerts in a simple but very powerful way, only available using SignalFx.

I can see that based on my current settings, the amount of alerts I would’ve received in 1 day would've been around 18.

To read more about Detector Previews, please visit this link:
https://docs.signalfx.com/en/latest/detect-alert/set-up-detectors.html#previewing-the-results-of-a-detector

Click on Proceed to Alert Message

In Severity choose Major

![](../images/M1-l2-7.png)  

Click on Proceed to Alert Recipients

Click on Add Recipient and then on your email displayed as the first option

![](../images/M1-l2-8.png)   

That's the same as entering that email address
OR you can enter another email address by clicking on E-mail...

That's just one example of the many Notification Services SignalFx has available
You can check this out by going to the INTEGRATIONS tab of the top menu, and see Notification Services 

Click on Proceed to Alert Activation

In Activate...click on Activate Alert Rule

![](../images/M1-l2-9.png)  
 
If you want to get alerts quicker you can click back on Alert Settings and lower the value from 290 to say 280.
If you change the Time to 1h you can see how many alerts you will be getting with the threshold you have chosen based on the metics from the last 1 hour.

Hover over ALERTS in the top menu and then click on Detectors

![](../images/M1-l2-10.png) 

You will see you alert detector listed here.

![](../images/M1-l2-11.png) 

Congrats! You have created your first alert detector and activated it!

***
Continue the workshop with [Working with Muting Rules](https://signalfx.github.io/app-dev-workshop/module1/muting/)