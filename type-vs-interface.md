# Type Alias vs Interface in TypeScript

## Introduction

TypeScript uses Type Alias and Interface to describe the shape of data. Both help developers write clean and safe code. They look similar, but they have some differences.

## What is Type Alias?

A Type Alias allows us to create a new name for a type. We can use it for objects, strings, numbers, unions, and many other types.

Example:

type Student = {
name: string;
age: number;
};

const student: Student = {
name: "Asrafuz",
age: 22,
};

Here, `Student` is a custom type. We can use it whenever we need the same structure.

## What is Interface?

An Interface describes the structure of an object. It tells us which properties an object should have.

Example:

interface Teacher {
name: string;
subject: string;
}

const teacher: Teacher = {
name: "Rahim",
subject: "English",
};

Here, the `Teacher` interface requires a name and a subject.

## Main Differences

Type Alias and Interface both support object types. However, an Interface can be extended using the `extends` keyword. Type Alias can also combine types using unions and intersections.

For example, we can use `type` to create a type like `string | number`.

## Conclusion

Type Alias and Interface are both useful in TypeScript. I can use Interface for object structures and Type Alias for unions and other complex types. Both help make code easier to understand and maintain.
