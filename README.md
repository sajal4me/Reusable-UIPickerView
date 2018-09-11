# Reusable-UIPickerView
Custom reusable Picker view completely written in swift 4

Usages:-

Multi Picker can be use either for 1 row or 2

for 1 components:-
let firstArray ["One", "Two", "Three", "Four", "Five"]
func textFieldShouldBeginEditing(_ textField: UITextField) -> Bool {

MultiPicker.noOfComponent = 1
MultiPicker.openMultiPickerIn(textField, firstComponentArray: firstArray, secondComponentArray: [""], firstComponent: "", secondComponent: nil, titles: nil) { (data, response, index) in


textField.text =  data
print(index)

}
