# jGenderize

Client for http://genderize.io web service.

Simple Java extension to know the gender of a given name.

What is the gender for "John" ?

```java
Genderize api = GenderizeIoAPI.create();
NameGender gender = api.getGender("John");
System.out.println("John is: "+gender.getGender());
System.out.println("is John male? " + gender.isMale());
System.out.println("Who? " + gender.getName());
```
What about "John" in Brazil? Localization support.

```java
Genderize api = GenderizeIoAPI.create();
NameGender gender = api.getGender("John", new Locale("pt", "BR");
System.out.println("John is: "+gender.getGender());
System.out.println("is John male? " + gender.isMale());
```
