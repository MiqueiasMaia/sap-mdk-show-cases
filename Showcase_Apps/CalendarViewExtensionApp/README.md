# Calendar View Extension App

This is a showcase application that demonstrates how to implement the Calendar View for Android as Extension Control.

*Last Updated: 05-Dec-2021*

### Author
* Robin Kuck ([GitHub](https://github.com/robinkuck), [SAP Community](https://people.sap.com/kucki99))

***

## Requirements

### Supported Platforms

* Android

### MDK Client Version

* MDK 6.1 or higher

### Data Source

* Mobile Services Sample OData ESPM (destination created as SampleServiceV2)

***

## Key Highlights

* Filtering of Object Table by selected date using implementation of Extensions `OnValueChange` event. This event is currently not supported in the layout editor, open the `Calendar.page` in code editor to access it. 
    >You might not see any Sales Orders in the table. Read below on how to add additional Sales Orders)
* Native control used: [Android CalendarView](https://developer.android.com/reference/android/widget/CalendarView)

## To Do

* Add implementation of native [FUICalendarView](https://help.sap.com/doc/978e4f6c968c4cc5a30f9d324aa4b1d7/Latest/en-US/Documents/Frameworks/SAPFiori/Classes/FUICalendarView.html) Control for iOS

***

## Setup Instructions

No additional steps required. The content of [CalendarViewExtensionApp/](CalendarViewExtensionApp/) folder can be used as is to run the application.

### Generate additional Sales Orders for current date

You can generate Sales Orders which are displayed in the Object Table after the application started. (The date filter is executed on the `CreatedAt` attribute of SalesOrderHeaders) 

In the app configuration of SAP Mobile Services cockpit, select the `Mobile Sample OData ESPM` feature:

<img src="Screenshots/generate_sales_orders1.png" width="95%">

Select `Generate sample sales orders`:

<img src="Screenshots/generate_sales_orders2.png" width="95%">

In the mobile application, select `Sync` to synchronize offline store and download the generated Sales Orders:

<img src="Screenshots/sync.png" width="35%">

## Screenshots

<img src="Screenshots/android.gif" width="35%">
