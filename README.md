[![Pub](https://img.shields.io/badge/Pub-0.1.2-orange.svg?style=flat-square)](https://pub.dartlang.org/packages/flutter_country_picker)

# flutter_country_picker
A Flutter Country Picker Widget with support to country dialing codes

<img src="https://github.com/biessek/flutter_country_picker/blob/master/example/img/1.png?raw=true" width="200"/>  
<img src="https://github.com/biessek/flutter_country_picker/blob/master/example/img/2.png?raw=true" width="200"/>

## Usage

Add the CountryPicker widget in your layout and use the `onChanged` callback.  
[Full example](https://github.com/biessek/flutter_country_picker/tree/master/example)

 ```dart

  @override
  Widget build(BuildContext context) {
    return new Scaffold(
      appBar: new AppBar(
        title: Text('Flutter Country Picker Demo'),
      ),
      body: new Center(
        child: CountryPicker(
          onChanged: (Country country) {
            setState(() {
              _selected = country;
            });
          },
          selectedCountry: _selected,
        ),
      ),
    );
  }

 ```