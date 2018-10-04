---
layout: post
title:  "My Swift Cheat Sheet"
date:   2018-09-17 4:38:53 -0600
categories: [ Mobile-Apps ]
---

# Swift Notes

## Include numbers in text
```swift
  let apples = 3
  let appleSummary = "I have \(apples) apples."
```
## Optionals

An optional value either contains a value or contains `nil` to indicate that the value is missing. Optionals are denoted by a `?` after a variables type.

```javascript
  var optionalName: String?
  var greeting = "Hello!"
  if let name = optionalName {
      greeting = "Hello, \(name)"
  }
```


If the optional value is `nil`, the conditional is `false` and the code in braces is skipped. Otherwise, the optional value is unwrapped and assigned to the constant after `let`, which makes the unwrapped value available inside the block of code.

#### Use `??` for default values
```swift
  let nickName: String? = nil
  let fullName: String = "John Appleseed"
  let informalGreeting = "Hi \(nickName ?? fullName)"
```

## Tuples
```swift
let violet = ("#EE82EE", 230, 130, 238
print("Violet is \(violet.0)")
let (hex, red, green, blue) = violet
print("Violet is \(hex)")
```

## Dictionaries
```swift
let elements = [
        ["title": "Color",
         "description": "some stuff about color",
         "image": "color"
        ],
        ["title": "Diagram",
         "description": "some stuff about diagram",
         "image": "diagram"
        ],
    ]
```

## Ranges
```swift
let rangesInfinite = 1...       // Infinite values
rangesInfinite.contains(3)      // true
rangesInfinite.contains(569999) // true
rangesInfinite.contains(0)      // false

let numbers = [1,2,3,4,5,6,7,8,9,10]
numbers[..<5]
```

## Loops
Use `..<` or `...` to create a range
```swift
  var total = 0
  for i in 0..<4 {
      total += i
  }
  print(total)
```

## Functions

Nested Functions have access to variables declared in the outer function


A function can take another function as an argument
  ```swift
  func hasAnyMatches(list: [Int], condition: (Int) -> Bool) -> Bool {
      for item in list {
          if condition(item) {
              return true
          }
      }
      return false
  }
  func lessThanTen(number: Int) -> Bool {
      return number < 10
  }
  var numbers = [20, 19, 7, 12]
  hasAnyMatches(list: numbers, condition: lessThanTen)
  ```
  
Functions are actually a kind of closure (blocks of code that can be called later). The code in a closure has access to things like variables and functions that were available in the scope where the closure was created, even if the closure is in a different scope when it is executed. A closure is denoted by braces `{}`. The `in` keyword is kinda like the `=>` in JS
  
```swift
numbers = [1, 2, 3, 4]
numbers.map({ (number: Int) -> Int in
    let result = 3 * number
    return result
})
```

When types of clusures are already known, you can omit them

```swift
let mappedNumbers = numbers.map({ number in 3 * number })
```

Closure parameters can be refered to by number
```swift
let sortedNumbers = numbers.sorted { $0 > $1 }
```