---

# What's New in 
# HealthKit
# ResearchKit and
# CareKit

---

# What's New in Health

---

***Don't get too excited***

![](https://media.giphy.com/media/26AHLspJScv2J6P0k/giphy.gif)

---

A bunch of things that don't matter to us
- Support for new workout types
- A lot of new features for swimming
- New Workout API updates including workout routes
- Sync data now includes identifiers and versioning

---

***What really matters***

![](https://media.giphy.com/media/UlT6oxzi1v2g0/giphy.gif)

---

***Supporting Diabetes Management***

- Blood glucose meal time

```
public let HKMetadataKeyBloodGlucoseMealTime: String
public enum HKBloodGlucoseMealTime: Int {
 case preprandial
 case postprandial
}
```
---

- Insulin delivery

```
public static let insulinDelivery: HKQuantityTypeIdentifier
public let HKMetadataKeyInsulinDeliveryReason: String
public enum HKInsulinDeliveryReason : Int {
 case basal
 case bolus
}
```
---

watchOS 4 supports CoreBluetooth

![](https://media.giphy.com/media/jVStxzak9yk2Q/giphy.gif)

---

# What's New in ResearchKit

---

![](http://www.troll.me/images/arnold-disgusting/whats-that-.jpg)

---

- Open source framework.
- Build surveys for medical research.
- Recruit partipants to take surveys or to just provide data.
- It is linked with HealthKit

---

![](http://blog.zuehlke.com/wp-content/uploads/2015/07/Slide5-755x334.png)

---

# What's New in ResearchKit

- Tone Audiometry - Hearing test
- Stroop test - Selective attention test
- Trail making test - neuro psychological test
- Range of Motion - Measure flexed and extended positions

---

# What's CareKit

- Open source framework
- Evolved from ResearchKit
- Great for cronic (ex: mental health) and acute (ex: surgery recovery) use cases
- It is linked with HealthKit
- Can use ResearchKit to assess the patient.

---

![](http://blog.shazino.com/imgs/articles/dev/carekit-introduction/carekit-screens.png)

- Care Card - displays treatment plan and progress
- Symptom Tracker - record measurements
- Insights - displays trends and gaps in patient care
- Connect - share data with family members or healthcare team
---

# What's New in CareKit

- Care Contents - combine Care Card with Symptom Tracker
- Configure thresholds in the assessments that will trigger alerts when something is above it.
- Chat to connect with healthcare providers

---

![](http://a.memegen.com/2cj5nl.gif)

---

# Questions?

![](http://3.bp.blogspot.com/-GWMIlb455pg/VOvngWloxnI/AAAAAAAAGZQ/xibdXIzAJJE/s1600/Is+Anyone+Listening+Meme.PNG)

