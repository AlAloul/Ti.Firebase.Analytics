Ti.Firebase.Analytics
=====================
This is Titanium module for realising of [tracking of app events by firebase.analytics](https://support.google.com/adwords/answer/6366292?hl=en).

This repo is in planning!

Please follow the howto from google above. For binding to your account you have to generate a google-services.json on google api console and copy to you Resources folder.

Here are instructions on youtube: https://www.youtube.com/watch?v=3UkLMcegenk

Usage/interface
---------------
```javascript
Ti.App.FirebaseAnalytics = require("ti.firebase.analytics");
// ………

Ti.App.FirebaseAnalytics.sendEvent({
	Ti.App.FirebaseAnalytics.ANALYTICS_ITEM_ID : "39836299",
	Ti.App.FirebaseAnalytics.ANALYTICS_ITEM_NAME : "39836299",
	Ti.App.FirebaseAnalytics.ANALYTICS_TAX : "39836.99",
	Ti.App.FirebaseAnalytics.ANALYTICS_PRICE : "39836.99",
	Ti.App.FirebaseAnalytics.ANALYTICS_ITEM_LOCATION_ID : "39836.99", // Google Place ID
	Ti.App.FirebaseAnalytics.ANALYTICS_LEVEL : "39836.99", // Level in game (long).
	Ti.App.FirebaseAnalytics.ANALYTICS_LOCATION : "3983699",
	campaignDetails : {
		Ti.App.FirebaseAnalytics.CAMPAIGN_DETAIL_ACLID : "9e293283",
		Ti.App.FirebaseAnalytics.CAMPAIGN_DETAIL_CAMPAIGN : "9e293283",
		Ti.App.FirebaseAnalytics.CAMPAIGN_DETAIL_CONTENT : "9e293283",
		Ti.App.FirebaseAnalytics.CAMPAIGN_DETAIL_CP1 : "9e293283",
		Ti.App.FirebaseAnalytics.CAMPAIGN_DETAIL_MEDIUM : "9e293283",
		Ti.App.FirebaseAnalytics.CAMPAIGN_DETAIL_SOURCE : "9e293283",
		Ti.App.FirebaseAnalytics.CAMPAIGN_DETAIL_TERM : "9e293283"
	}
});

```
You can use all paramters from this [documentation](https://firebase.google.com/docs/reference/android/com/google/firebase/analytics/FirebaseAnalytics.Param)
