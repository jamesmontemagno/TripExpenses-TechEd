Xamarin.Forms-TripExpenses
==========================

Xamarin.Forms Azure Demo of a simple expense app with Azure Mobile Services online and offline sync with a backed SQLite database for iOS, Android, and Windows Phone.

##Setup

* By default TripExpenses uses a cross-platform Json Based file system, however you can add Azure Mobile Services easily by following:

* Signup for an Azure Mobile Services account: https://azure.microsoft.com/services/mobile-services/?WT.mc_id=tripexpenses.forms-github-jamont
* Open: XMLDataStore.cs and comment OUT the [assemby:Dependency()] flag
* Create a new Azure Mobile Services Table Called "TripExpense"
* Open “AzureDataStore.cs" in TripExpenses shared project
* Comment IN the [assemby:Dependency()] flag
* Edit: MobileService = new MobileServiceClient(
        "https://"+"PUT-SITE-HERE" +".azure-mobile.net/",
        "PUT-YOUR-API-KEY-HERE");


##Watch

* Full Session on Channel 9: https://channel9.msdn.com/Events/dotnetConf/2014/Developing-Native-iOS-Android-and-Windows-Apps-with-Xamarin?WT.mc_id=tripexpenses.forms-github-jamont
* Slides available: http://www.slideshare.net/JamesMontemagno/dotnetconf-introduction-to-xamarin-and-xamarinforms