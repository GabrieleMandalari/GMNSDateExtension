GMNSDateExtension
=================

GMNSDateExtension is a simple Objective-C library designed to extend some functions of NSDate class.


<h2><b>Setup</b></h2>

To use GMNSDateExtension in your project copy "Library" folder and import just one file:

`#import "GMNSDateExtension.h"`

<h2><b>How To Use</b></h2>

Each method takes a parameter that specifies the format for each date. Example:

`+(NSDate*) dateFromString: (NSString*) date withFormat: (NSString*) format`

</br>

The format is your choice: `@"yyyy-MM-dd` `@"dd-MM-yyyy` ecc

</br>

But you can also use a standar format with:

`[GMNSDateExtension dateFormat:DateFormatAmerican]`

or

`[GMNSDateExtension dateFormat:DateFormatEuropean]`

</br>

<h2><b>Example to use</b></h2>

Examples to get day component from a generic date or yesterday/tomorrow date:

`NSInteger dayComponent = [GMNSDateExtension dayComponenetFromDate:[NSDate date] withFormat:@"dd-MM-yyyy"];`

`NSDate *tomorrow = [GMNSDateExtension dateTomorrowWithFormat: [GMNSDateExtension dateFormat: DateFormatEuropean]];`
	
`NSDate *yesterday = [GMNSDateExtension dateYesterdayWithFormat: [GMNSDateExtension dateFormat: DateFormatEuropean]];`


</br>	



<h2><b>Methods</b></h2>

Determines if an NSDate is today

`+(BOOL) isToday: (NSDate*) date withFormat:(NSString*) format;`

</br>

Determines if an NSDate is yesterday

`+(BOOL) isYesterday: (NSDate*) date withFormat:(NSString*) format;`

</br>

Determines if an NSDate is tomorrow

`+(BOOL) isTomorrow: (NSDate*) date withFormat:(NSString*) format;`

</br>

Get the Tommorrow date

`+(NSDate *) dateTomorrowWithFormat:(NSString*) format;`

</br>

Get the Yesterday date

`+(NSDate *) dateYesterdayWithFormat:(NSString*) format;`

</br>

Convert NSString to NSDate

`+(NSDate*) dateFromString: (NSString*) date withFormat: (NSString*) format;`

</br>

Convert  NSDate to NSString

`+(NSString*) stringFromDate: (NSDate*) date withFormat: (NSString*) format;`

</br>

Get NSdateComponents from NSString

`+(NSDateComponents*) dateComponentsFromString: (NSString*) date withFormat: (NSString*) format;`

</br>

Get NSdateComponents from NSDate

`+(NSDateComponents*) dateComponentsFromDate: (NSDate*) date withFormat: (NSString*) format;`

</br>

Get year, month, day, hour, minute or seconds from NSDate

`+(NSInteger) yearComponentFromDate:(NSDate*) date withFormat: (NSString*) format;`

`+(NSInteger) monthComponenetFromDate:(NSDate*) date withFormat: (NSString*) format;`

`+(NSInteger) dayComponenetFromDate:(NSDate*) date withFormat: (NSString*) format;`

`+(NSInteger) hourComponenetFromDate:(NSDate*) date withFormat: (NSString*) format;`

`+(NSInteger) minuteComponenetFromDate:(NSDate*) date withFormat: (NSString*) format;`

`+(NSInteger) secondComponenetFromDate:(NSDate*) date withFormat: (NSString*) format;`

</br>


Get year, month, day, hour, minute or seconds from NSString

`+(NSInteger) yearComponenetFromString:(NSString*) date withFormat: (NSString*) format;`

`+(NSInteger) monthComponenetFromString:(NSString*) date withFormat: (NSString*) format;`

`+(NSInteger) dayComponenetFromString:(NSString*) date withFormat: (NSString*) format;`

`+(NSInteger) hourComponenetFromString:(NSString*) date withFormat: (NSString*) format;`

`+(NSInteger) minuteComponenetFromString:(NSString*) date withFormat: (NSString*) format;`

`+(NSInteger) secondComponenetFromString:(NSString*) date withFormat: (NSString*) format;`

</br>


Get difference between two NSDate

`+(NSInteger) yearsDifferenceFromDate:(NSDate*) fromDate toDate: (NSDate*) toDate withFormat: (NSString*) format;`

`+(NSInteger) monthsDifferenceFromDate:(NSDate*) fromDate toDate: (NSDate*) toDate withFormat: (NSString*) format;`

`+(NSInteger) daysDifferenceFromDate:(NSDate*) fromDate toDate: (NSDate*) toDate withFormat: (NSString*) format;`

`+(NSInteger) hoursDifferenceFromDate:(NSDate*) fromDate toDate: (NSDate*) toDate withFormat: (NSString*) format;`

`+(NSInteger) minuteDifferenceFromDate:(NSDate*) fromDate toDate: (NSDate*) toDate withFormat: (NSString*) format;`

`+(NSInteger) secondsDifferenceFromDate:(NSDate*) fromDate toDate: (NSDate*) toDate withFormat: (NSString*) format;`

`+(NSString*) dateFormat:(DateFromat) dateformat;`


<h2><b>Suggestions</b></h2>

Contatc me to mandalari.gabriele@gmail.com to add other methods
