# Note
Edit and rebuild of #react-native-multiple-select-list(https://github.com/ataomega/react-native-multiple-select-list)
Thanks for author

# react-native-multiple-select-list
Multiple select list with search bar

### Install :
```sh
npm install --save react-native-multiple-select-list-rebuild
```
### Example usage :
```javascript
import CustomMultiPicker from "react-native-multiple-select-list";

const userList = {
  "123":"Tom",
  "124":"Michael",
  "125":"Christin"
}

<CustomMultiPicker
  options={this.props.data}
  search={true} // should show search bar?
  multiple={true} //
  placeholder={"Search"}
  reminderSearch={"Search để có dữ liệu"}
  placeholderTextColor={'#757575'}
  returnValue={"value"} // label or value
  isOption={true} // show panel option
  callback={(res) => this.setState({ dataSelected: res })}
  rowBackgroundColor={"#eee"}
  rowHeight={40}
  rowRadius={5}
  iconColor={"#00a2dd"}
  iconSize={30}
  selectedIconName={"ios-checkmark-circle-outline"}
  unselectedIconName={"ios-radio-button-off-outline"}
  scrollViewHeight={'100%'}
  selected={this.state.selected}
/>
```

![react-native-multiple-select-list](https://raw.githubusercontent.com/ataomega/react-native-multiple-select-list/master/screenshot.png)


### Props:
| Prop | Type | Description |
| ------ | ------ | ------ |
| options | Object | list of options/items |
| search | Boolean | if the search bar should be shown or not |
| multiple | Boolean | if user can select multiple options or not. if you select an item which is already selected, it will be unselected. if multiple is disabled, it will work like radio buttons. |
| placeholder | String | placeholder text for search bar |
| placeholderTextColor | String | placeholder text color for search bar |
| reminderSearch | String | reminder search |
| isOption | Boolean | panel more option |
| returnValue | String | should it return keys of selected options or values? |
| callback | Function | whenever user selects or changes selections it will be called. |
| rowBackgroundColor | String | background color for each row in list |
| rowHeight | Integer | row height |
| rowRadius | Integer | row border radius |
| iconColor | String | icon color for checked/unchecked icons and search icon also border color of search bar |
| iconSize | Integer | icon size for checked/unchecked icons |
| selectedIconName | String | selected/checked icon name (react-native-vector-icons/Ionicon) |
| unselectedIconName | String | unselected/unchecked icon name (react-native-vector-icons/Ionicon) |
| scrollViewHeight | Integer |scrollview height (list of items) |
| selected | Object | list of options which are selected by default |

### Author:
stock source: ataomega@gmail.com
re-change: damdinhhuy@gmail.com
# rn-multiple-select-list-rebuild
