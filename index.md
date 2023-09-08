# This is Heading 1 `<h1>`
## This is Heading 2 `<h2>`
### This is Heading 3 `<h3>`
#### This is Heading 4 `<h4>`
##### This is Heading 5 `<h5>`
###### This is Heading 6 `<h6>`

![Image of El Capitan, Bridalveil Falls, and Merced River](https://a.cdn-hotels.com/gdcs/production126/d349/d2422886-1662-43cb-a356-4087bdbb59f8.jpg)

```swift
struct Reset: Codable, Identifiable {
    let resetType: String
    let user: User
    let id = UUID()
   // let resetType: resetType
    let otherVendorsPresent: Bool
    let account: Account
    let scheduledDaate: Date
    var locationLattitude: CLLocationCoordinate2D?{
        if account.location != nil{
            return account.location
        }
        return nil
    }
    let coldVaultBeforeNumbers: ColdVaultBeforeNumbers?
    let warmBeforeNumbers: WarmBeforeNumbers?
    let warmAfterNumbers: WarmAfterNumbers?
    let coldVaultAfterNumbers: ColdVaultAfterNumbers?
    let resetIsComplete: Bool = false
    let pdfData: Data?
    let glidesUsed: GlideTacker?
}
```

- [x] Create Reset struct
- [x] Create stored properties
- [ ] Setup Core Data
