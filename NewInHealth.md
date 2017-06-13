---

<!-- footer: Powered by babylon health -->

# What's New in Health

---

Don't get too excited

![](https://media.giphy.com/media/26AHLspJScv2J6P0k/giphy.gif)

---

A bunch of things that don't matter to us
- Support for new workout types
- A lot of new features for swimming
- New Workout API updates including new data type -> routes
- Sync data now includes identifiers and versioning

---

What really matters

![](https://media.giphy.com/media/UlT6oxzi1v2g0/giphy.gif)

---

Supporting Diabetes Management

- Blood glucose meal time
```

public let HKMetadataKeyBloodGlucoseMealTime: String
public enum HKBloodGlucoseMealTime: Int {
 case preprandial
 case postprandial
}
```
---

Supporting Diabetes Management

- Insulin delivery

```

public static let insulinDelivery: HKQuantityTypeIdentifier
public let HKMetadataKeyInsulinDeliveryReason: String
public enum HKInsulinDeliveryReason : Int {
 case basal
 case bolus
}
```
