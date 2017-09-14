# React Native Tips

### Fonts
Adding custom fonts to an Android project:
- copy your .ttf fonts to /android/app/src/main/assets/fonts
- rename your fonts to be all lower case and no spaces: Roboto Light.ttf will be robotolight.ttf
- in your js file use the font as follows:
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
