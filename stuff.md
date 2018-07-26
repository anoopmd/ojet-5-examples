Validators & Converters
=======================

Oracle JET provides the oj.Validation class which includes methods to register and retrieve converter and validator factories.

You can provide a custom factory that implements the contract for a converter using oj.ConverterFactory or a validator using oj.ValidatorFactory and register the converter or validator with the oj.Validation class.

The oj.Validation class enables you to access your custom converter or validator using the same mechanisms as you would use with the Oracle JET standard converters and validators.

Validators
==========
All Oracle JET editable elements support a value attribute and provide UI elements that allow the user to enter or choose a value. These elements also support other attributes that page authors can set that instruct the element how it should validate its value.

An editable element may implicitly create a built-in converter and/or built-in validators for its normal functioning when certain attributes are set.

For example, editable elements that support a required property create the required validator implicitly when the property is set to true. Other elements like oj-input-date, oj-input-date-time, and oj-input-time create a datetime converter to implement its basic functionality.

There are 6 validators given by OJET
1. oj.DateTimeRangeValidator - Validates that the input date is between two dates, between two times, or within two date and time ranges
2. oj.DateRestrictionValidator - Validates that the input date is not a restricted date
3. oj.LengthValidator - Validates that an input string is within a specified length
4. oj.NumberRangeValidator - Validates that an input number is within a specified range
5. oj.RegExpValidator - Validates that the regular expression matches a specified pattern
6. oj.RequiredValidator - Validates that a required entry exists

About Converters
The Oracle JET converters include
oj.ColorConverter - Converts oj.Color object formats
oj.IntlDateTimeConverter - Converts a string to a Date or a Date to a string
oj.IntlNumberConverter - Converts a string to a number or formats a number or Number object value to a string










