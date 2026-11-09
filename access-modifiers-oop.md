# Access Modifiers in Object-Oriented Programming

## Introduction

Access Modifiers are an important part of Object-Oriented Programming (OOP). They control where we can access class properties and methods. TypeScript has three main access modifiers: public, private, and protected.

## 1. Public

Public members can be accessed from anywhere. It is the default access modifier in TypeScript.

Example:

class Student {
public name: string = "Asrafuz";
}

const student = new Student();
console.log(student.name);

Here, we can access the name from outside the class.

## 2. Private

Private members can only be accessed inside their own class. We cannot directly access them from outside the class or from a child class.

Example:

class Bank {
private balance: number = 5000;
}

Here, the balance is private. It helps protect important data.

## 3. Protected

Protected members can be accessed inside their own class and its child classes. However, we cannot access them directly from outside the class.

Example:

class Person {
protected name: string = "Rahim";
}

class Employee extends Person {
showName(): string {
return this.name;
}
}

Here, the Employee class can access the protected name because it extends the Person class.

## Conclusion

Access Modifiers help us control access to class data. Public is open to everyone, private is only for its own class, and protected is available to its own class and child classes. They help us write safer and more organized code.
