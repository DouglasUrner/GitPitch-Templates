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

@[3](Declare & initialize an array)
@[5](Assign to an element of the array)
@[7-11](Loop over the array using an index)
@[13-17](Iterate over all the items in the array using a "foreach loop" – no index.)

Note:

---

## The List Interface

---

## ArrayList

```java
List<EmailAddress> emailAddresses =
  new ArrayList<>();

emailAddresses.add(7, new EmailAddress("me@example.com"));

emailAddresses.add(new EmailAddress("you@example.com"));

for (int i = 0; i < size; i++) {
  if (emailAddresses.get(i) != null) {
    System.out.println(emailAddresses.get(i));
  }
}

for (EmailAddress e : emailAddresses) {
  if (e != null) {
    System.out.println(e);
  }
}
```

@[1-2](Declare & initialize an ArrayList)
@[4](Assign to a specific position in the list (7))
@[6](Assign to the next available position in the list)
@[8-12](Loop over the list using an index)
@[14-18](Iterate over all the items in the list using a "foreach loop" – no index.)

Note:
No need to specify the size of the list - it will grow as necessary.
You may see examples with the type listed on both sides of the declaration, but this is not needed in recent versions of Java.
