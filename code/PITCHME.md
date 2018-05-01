---?image=images/margaret-hamilton-with-apollo-listings-665x1200.jpg&position=left&size=auto 100%

## Working With Collections of Objects

Note:

Margaret Hamilton, the lead software engineer on the team that wrote the code for the guidance computer of the Apollo lunar excursion module standing next to a stack the listings of their code. Cambridge, MA - 1969.

---

## Arrays

```java
int size = 42;

EmailAddress[] emailAddresses = new EmailAddress[size];

emailAddresses[7] = new EmailAddress("me@example.com");

for (int i = 0; i < size; i++) {
  if (emailAddresses[i] != null) {
    System.out.println(emailAddresses[i]);
  }
}

for (EmailAddress e : emailAddresses) {
  if (e != null) {
    System.out.println(e);
  }
}
```

@[3](Declare & Initialize An Array)
@[5](Assign To An Element Of The Array)
@[7-11](Loop Over The Array Using An Index)
@[13-17](Use a "foreach loop" to iterate over all of the items in the list.)

---

## The List Interface

---

## ArrayList
