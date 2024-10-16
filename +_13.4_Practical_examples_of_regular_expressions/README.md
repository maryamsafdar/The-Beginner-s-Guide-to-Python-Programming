<p><strong>Chapter 13.4: Practical Examples of Regular Expressions</strong></p>

<p>Regular expressions are a powerful tool for text manipulation and analysis. In this chapter, we will explore 13 practical examples of regular expressions, covering a wide range of scenarios, from simple text matching to complex pattern extraction.</p>

<p><strong>Example 1: Validating Email Addresses</strong></p>

<p>Email addresses are a common requirement in many applications. We can use regular expressions to validate email addresses and ensure they conform to a standard format.</p>

<p><code>regex
^[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$
</code></p>

<p>This regular expression matches most common email address formats, including those with special characters and top-level domains.</p>

<p><strong>Example 2: Extracting Phone Numbers</strong></p>

<p>Phone numbers can be extracted from text using regular expressions. We can match various formats, including international numbers and numbers with extensions.</p>

<p><code>regex
\(?([0-9]{3})\)?[-. ]?([0-9]{3})[-. ]?([0-9]{4})|([0-9]{10})
</code></p>

<p>This regular expression matches phone numbers in the format (123) 456-7890, 123-456-7890, or 1234567890.</p>

<p><strong>Example 3: Validating Passwords</strong></p>

<p>Password validation is an essential security measure. We can use regular expressions to enforce password policies, such as minimum length, uppercase letters, and special characters.</p>

<p><code>regex
^(?=.*[a-z])(?=.*[A-Z])(?=.*\d)(?=.*[@$!%*#?&amp;])[A-Za-z\d@$!%*#?&amp;]{8,}$
</code></p>

<p>This regular expression matches passwords that contain at least one lowercase letter, one uppercase letter, one digit, and one special character, with a minimum length of 8 characters.</p>

<p><strong>Example 4: Extracting Dates</strong></p>

<p>Dates can be extracted from text using regular expressions. We can match various formats, including MM/DD/YYYY, DD/MM/YYYY, and YYYY-MM-DD.</p>

<p><code>regex
(\d{1,2}/\d{1,2}/\d{4})|(\d{1,2}-\d{1,2}-\d{4})|(\d{4}-\d{1,2}-\d{1,2})
</code></p>

<p>This regular expression matches dates in the format MM/DD/YYYY, DD/MM/YYYY, or YYYY-MM-DD.</p>

<p><strong>Example 5: Validating Credit Card Numbers</strong></p>

<p>Credit card numbers can be validated using regular expressions. We can match various formats, including Visa, Mastercard, and American Express.</p>

<p><code>regex
^4[0-9]{12}(?:[0-9]{3})?$|^5[1-5][0-9]{14}$|^3[47][0-9]{13}$
</code></p>

<p>This regular expression matches Visa, Mastercard, and American Express credit card numbers.</p>

<p><strong>Example 6: Extracting IP Addresses</strong></p>

<p>IP addresses can be extracted from text using regular expressions. We can match various formats, including IPv4 and IPv6.</p>

<p><code>regex
^((25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$|^([a-fA-F0-9]{1,4}:){7}[a-fA-F0-9]{1,4}$
</code></p>

<p>This regular expression matches IPv4 and IPv6 addresses.</p>

<p><strong>Example 7: Validating URLs</strong></p>

<p>URLs can be validated using regular expressions. We can match various formats, including HTTP and HTTPS.</p>

<p><code>regex
^(http|https)://[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}(:[a-zA-Z0-9]+)?(/.*)?$
</code></p>

<p>This regular expression matches HTTP and HTTPS URLs.</p>

<p><strong>Example 8: Extracting Social Security Numbers</strong></p>

<p>Social Security numbers can be extracted from text using regular expressions. We can match various formats, including XXX-XX-XXXX and XXXXXXXXXX.</p>

<p><code>regex
^\d{3}-\d{2}-\d{4}$|^(\d{9})$
</code></p>

<p>This regular expression matches Social Security numbers in the format XXX-XX-XXXX or XXXXXXXXXX.</p>

<p><strong>Example 9: Validating ZIP Codes</strong></p>

<p>ZIP codes can be validated using regular expressions. We can match various formats, including 5-digit and 9-digit codes.</p>

<p><code>regex
^\d{5}(-\d{4})?$|^(\d{9})$
</code></p>

<p>This regular expression matches 5-digit and 9-digit ZIP codes.</p>

<p><strong>Example 10: Extracting Time Zones</strong></p>

<p>Time zones can be extracted from text using regular expressions. We can match various formats, including UTC and GMT.</p>

<p><code>regex
^(UTC|GMT)(\+|-)(\d{1,2}):(\d{2})$
</code></p>

<p>This regular expression matches time zones in the format UTC+HH:MM or GMT+HH:MM.</p>

<p><strong>Example 11: Validating MAC Addresses</strong></p>

<p>MAC addresses can be validated using regular expressions. We can match various formats, including XXXX:XXXX:XXXX and XXXXXXXXX.</p>

<p><code>regex
^[0-9A-F]{2}:[0-9A-F]{2}:[0-9A-F]{2}:[0-9A-F]{2}:[0-9A-F]{2}:[0-9A-F]{2}$|^([0-9A-F]{12})$
</code></p>

<p>This regular expression matches MAC addresses in the format XXXX:XXXX:XXXX or XXXXXXXXX.</p>

<p><strong>Example 12: Extracting Currency Codes</strong></p>

<p>Currency codes can be extracted from text using regular expressions. We can match various formats, including USD and EUR.</p>

<p><code>regex
^USD|EUR|GBP|JPY|CNY|AUD|CAD|CHF|HKD|INR|MXN|NOK|NZD|RUB|SEK|SGD|ZAR$
</code></p>

<p>This regular expression matches currency codes.</p>

<p><strong>Example 13: Validating ISBNs</strong></p>

<p>ISBNs can be validated using regular expressions. We can match various formats, including 10-digit and 13-digit codes.</p>

<p><code>regex
^97[89][0-9]{10}$|^978[0-9]{10}$|^979[0-9]{10}$|^97[89][0-9]{13}$|^978[0-9]{13}$|^979[0-9]{13}$
</code></p>

<p>This regular expression matches ISBNs in the format 97XXX-XXXXX or 978XXX-XXXXX.</p>

<p>In conclusion, regular expressions are a powerful tool for text manipulation and analysis. By using the examples provided in this chapter, you can create robust and efficient solutions for a wide range of scenarios, from simple text matching to complex pattern extraction.</p>
