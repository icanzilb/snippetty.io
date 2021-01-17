# Simple Swift demo

In a new single view Xcode project open ViewController.swift.

Add a new property to `ViewController` class:

```swift
private var isSelected = false
```

Add a tap listener inside `viewDidLoad()`:

```swift
view.addGestureRecognizer(
    UITapGestureRecognizer(target: self, action: #selector(didTap))
)
```

Finally, add the tap handler method inside `ViewController` class:

```swift
@objc func didTap() {
    view.backgroundColor = isSelected ? .white : .red
    isSelected = !isSelected
}
```

Run the app and demo by repeatedly clicking the simulator.