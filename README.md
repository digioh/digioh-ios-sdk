# digioh-ios-sdk

## How to integrate Digioh.xcframework in your project

To add `Digioh.xcframework` to your iOS project follow below instructions:
1. Down `Digioh.xcframework` from repo.
2. Open your project
3. Drag & drop Digioh.xcframework manually into your project's target

Refer to the image below for further guidance on the steps.
![iOS Digioh Gif](https://user-images.githubusercontent.com/58115993/236928097-9c1847cb-3da1-44a0-a327-9d2f7de26c92.gif)

## How to get `Digioh Boxes`
```
import Digioh
let digioh = DigiohWeb(userGId: "Your api key")
digioh.checkShowBoxes(params: "", completion: @escaping (Result) -> Void)
```
- params if any pass in string otherwise `""
- will complete with `[UInt]` with boxes `id``

## Present `Digioh Boxes` in `Web View`
``
func showBox(boxId: UInt, viewController: UIViewController)
``
- pass box `ID`
- pass `ViewController` using `self`
