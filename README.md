# STTableBoard
☃️ A TableBoard that row can be moved everywhere just like Trello (for iPhone and iPad)
[Teambition](https://itunes.apple.com/cn/app/teambition/id656664814?l=en&mt=8) is using the STTableBoard.

### GIF
![image](https://raw.githubusercontent.com/StormXX/STTableBoard/master/GIF/STTableBoard.gif)

## Usage
1. Init a STTableBoard with `let table = STTableBoard(localizedStrings: yourLocalizedString)` 
2. RegisterClasses use `registerClasses(_ classAndIdentifier: [(AnyClass,String)])`
3. Set the delegate and dataSource to the UIViewController
3. Add it to SuperViewController 

```
self.addChildViewController(tableBoard)
view.addSubview(tableBoard.view)
tableBoard.didMove(toParentViewController: self)
```

4. (Download the **demo** and excute `carthage update` to run it

>  The TableBoard has two delagate: `STTableBoardDelegate` and `STTableBoardDataSource`, it's just like the delegate of UITableView

## Localization
You can do your localization for the tableboard.
**Example**: 

```
var localizedString: [String: String] = [
        "STTableBoard.AddRow": LocalizedString("AddRow"),
        "STTableBoard.AddBoard": LocalizedString("AddBoard"),
        "STTableBoard.BoardMenuTextViewController.Title": LocalizedString("BoardMenuTextViewController.Title"),
        "STTableBoard.EditBoardNameCell.Title": LocalizedString("EditBoardNameCell.Title"),
        "STTableBoard.DeleteBoardCell.Title": LocalizedString("DeleteBoardCell.Title"),
        "STTableBoard.DeleteBoard.Alert.Message": LocalizedString("DeleteBoard.Alert.Message"),
        "STTableBoard.Delete": LocalizedString("Delete"),
        "STTableBoard.Cancel": LocalizedString("Cancel"),
        "STTableBoard.OK": LocalizedString("OK"),
        "STTableBoard.Create": LocalizedString("Create"),
        "STTableBoard.RefreshFooter.text": LocalizedString("RefreshFooter.text")
    ]
```

## Minimum Requirement
iOS 8.0 

## License
STTableBoard is released under the CC license. See [Creative Commons](https://github.com/StormXX/STTableBoard/blob/master/LICENSE) for details.


## More Info
Have a question? Please [open an issue](https://github.com/StormXX/STTableBoard/issues/new)!


