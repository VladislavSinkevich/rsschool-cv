# Software developer resume

1. Vladislav Sinkevich
2. [email](mailto:vlad.sinkevich@gmail.com)
3. I want to change my main stack and work hard with new projects
4. Skills: HTML, CSS, JS, GIT
5. Code examples:

```
	public static void printBonusDatesBetween(int fromYear, int toYear) {
		GregorianCalendar dateFrom = new GregorianCalendar(fromYear, 0, 1);
		GregorianCalendar dateTo = new GregorianCalendar(toYear, 11, 31);

		DateFormat dateFormatResult = new SimpleDateFormat("yyyy-MM-dd");
		DateFormat dateFormatMonthDay = new SimpleDateFormat("MMdd");

		String currentDate;
		Boolean isPolindrom = false;
		int i = 0;
		int symbolCenter = 4;
		int maxSymbol = 7;

		while (0 >= dateFrom.compareTo(dateTo)) {

			currentDate = "" + dateFrom.get(GregorianCalendar.YEAR)
									+ dateFormatMonthDay.format(dateFrom.getTime());

			isPolindrom = true;

			maxSymbol = currentDate.length() - 1;
			symbolCenter = currentDate.length() / 2;

			for (i = 0; i < symbolCenter; i++) {
				if (currentDate.charAt(i) != currentDate.charAt(maxSymbol - i)) {
					isPolindrom = false;
				}
			};

			if (isPolindrom) {
				System.out.println(dateFormatResult.format(dateFrom.getTime()));
			};

			dateFrom.add(GregorianCalendar.DAY_OF_MONTH, 1);
		}

	}
```

6. Experience: since 2004 as 1C Organization developer
7. Education:
   - Vilnius University Computer Science
   - Udemy Web Development Bootcamp
8. English: AMES courses
