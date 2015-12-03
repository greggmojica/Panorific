Panorific
=========

**An immersive, intuitive, motion-based way to explore high-quality panoramas and photos on an iOS device. Panorific is implemented in Swift.**

<img src="screenshot.png" alt="Screenshot" width="320px"/>
<img src="preview.gif" alt="Preview" height="568px"/>


<!--## Installation
[CocoaPods](http://cocoapods.org) is the recommended method of installing Panorific. Simply add the following line to your `Podfile`:

#### Podfile

``` ruby
pod 'Panorific'
```
-->

## Requirements

- iOS 8.0+
- Xcode 7.0

## Usage

1. Skip this step if you're not using Storyboards. Drag a UIViewController from the Object Library onto the Storyboard and change its class to `PanorificViewController` in the Identity Inspector. Set the appropriate Auto Layout constraints.
2. In the presenting view controller's `prepareForSegue(_:sender:)`, set the `image` property of the appearing `PanorificViewController`.

``` Swift
override func prepareForSegue(segue: UIStoryboardSegue, sender: AnyObject?) {
    if segue.identifier == "ShowPanorificSegue" {
        let destination = segue.destinationViewController as PanorificViewController
        destination.image = UIImage(named: "BreathtakingImage")
    }
}
```

## Contact

Naji Dmeiri

- http://najidmeiri.com
- http://github.com/ndmeiri

## License

Panorific is available under the MIT License. See the LICENSE file for more info.
