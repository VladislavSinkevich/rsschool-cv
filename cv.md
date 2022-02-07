# Software developer resume

1. Vladislav Sinkevich
2. [email](mailto:vlad.sinkevich@gmail.com)
3. Summary (your goal, wishes, reveal what is important for you, what do you want and why.
   Some kind of self-presentation. In case of lack of experience Junior Developer sells his/her potential, his/her passion and ability to learn fast. You shouldn't think that everybody is going to teach you when you come to the workplace . Rather being a Junior means always
   learning new things from everywhere etc.).
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

			currentDate = "" + dateFrom.get(GregorianCalendar.YEAR) + dateFormatMonthDay.format(dateFrom.getTime());

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

6. Experience (for a Junior Dev it means all kinds of experience: coding tests, projects from courses,
   freelance projects - wherever they had the opportunity to demonstrate skills they have.
   Also it would be awesome if you add links to source code)
7. Education (including courses, seminars, lectures, online learning)
8. English (elaborate on what kind of practice you had, if any, how long it lasted and so on)
