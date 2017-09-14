# React Native Tips

### Fonts
Adding custom fonts to an Android project:
- copy your .ttf fonts to /android/app/src/main/assets/fonts
- rename your fonts to be all lower case and no spaces: Roboto Light.ttf will be robotolight.ttf
- in your js file use the font by adding the file name to the "fontFamily" style property:

```javascript
export default class AwesomeProject extends Component {
  render() {
    return (
        <View>
            <Text style={ styles.text }>
                Some text for testing
            </Text>
        </View>
    );
  }
}

const styles = StyleSheet.create({
    text: {
        color: "white",
        fontFamily: "robotolight",
        fontSize: 40
    }
}
```

### Interaction
Adding a touch event to a text element is done via the onPress event listener

```javascript
export default class AwesomeProject extends Component {
  render() {
    return (
        <View>
            <Text onPress={ () => this.doSomething() }>
                Some text for testing
            </Text>
        </View>
    );
  }
}
