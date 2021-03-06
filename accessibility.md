
<br>
# What’s new in Accessibility

![inline](https://developer.apple.com/accessibility/images/hero_accessibility.png)

<br>
<br>

^ Over 1 milion people have a disability 
	Cognitive
	Motor
	Vision
	Hearing

---

## New Assistive Features

---

### Text Detection

![inline](https://d2pu2bk1b66iw6.cloudfront.net/photos/2014/08/01/6-75097-mm_babymeme50-1406927589.jpg) 

---

### Improved Photo Description

![inline](https://s-media-cache-ak0.pinimg.com/736x/50/9c/6e/509c6ecc57c2fd7c79911d1b24c9447a--baby-beach-beach-babies.jpg)

---

### What's New In Dynamic Type

- Text large enough for the user to read
- Text not truncated or cropped
- Keeps a good UI experience

^ The tab bar long press shows a bigger icon in the middle of the screen representing the tab bar icon.

---

- Bigger fonts
- Supports custom fonts
- Keeps a good UI experience

^ The tab bar long press shows a bigger icon in the middle of the screen representing the tab bar icon.

---

### How to accomodate big fonts?

- Wrap the text

- Labels overlapping each other when using constants for spacing?

  Spacing between labels can be dynaminc using: 

```swift
secondLabel.firstBaselineAnchor
		   .constraintEqualToSystemSpacingBelow(firstLabel.lastBaselineAnchor, 
		   										multiplier: 1.0)
```

^ It changes the spacing automatically based on the font size

---

- Alternate layout

	For side by side labels with large text size the labels should be moved to a vertical stack
	
![inline, fit](https://raw.githubusercontent.com/AnnKatF/WWDC17Presentations/master/label_cropped.jpg)

![inline, fit](https://raw.githubusercontent.com/AnnKatF/WWDC17Presentations/master/label_vertical.jpg)

---

<br>
<br>
Example:

```swift
	if traitCollection.preferredContentSizeCategory > .extraExtraLarge { 
		// Vertically stack
	} else {
		// Lay out side by side
	}
```

---

Standard table view cells will handle it automatically.

![inline, fit](https://raw.githubusercontent.com/AnnKatF/WWDC17Presentations/master/tableview_layout.jpg)

---

- Allow Images to Scale Up

1. Images as PDF at 1x scale
2. Asset catalog enable `Preserve Vector Data`
3. Image view enable `Adjust Image Size`

```swift
imageView.adjustsImageSizeForAccessibilityContentSizeCategory = true
```

^ Preserve Vector Data prevents the pdf from being converted into png files for each scale.
Uses PDF drawing.

---

### UIAccessibility Protocol

![inline, fit](https://raw.githubusercontent.com/AnnKatF/WWDC17Presentations/master/access_0.jpg)

![inline, fit](https://raw.githubusercontent.com/AnnKatF/WWDC17Presentations/master/access_1.jpg)



