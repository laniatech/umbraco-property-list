﻿# Property List

[![Build status](https://img.shields.io/appveyor/ci/UMCO/umbraco-property-list.svg)](https://ci.appveyor.com/project/UMCO/umbraco-property-list)
[![NuGet release](https://img.shields.io/nuget/v/Our.Umbraco.PropertyList.svg)](https://www.nuget.org/packages/Our.Umbraco.PropertyList)

Property List is a property editor for making repeatable lists of a datatype for Umbraco 7.6+

## Getting Started

### Installation

> *Note:* Property List has been developed against **Umbraco v7.6.0** and will support that version and above.

Property List can be installed from either NuGet package repositories, or build manually from the source-code:


#### NuGet package repository

To [install from NuGet](https://www.nuget.org/packages/Our.Umbraco.PropertyList), you can run the following command from within Visual Studio:

	PM> Install-Package Our.Umbraco.PropertyList

We also have a [MyGet package repository](https://www.myget.org/gallery/umbraco-packages) - for bleeding-edge / development releases.
#### Manual build

If you prefer, you can compile Property List yourself, you'll need:

* Visual Studio 2017 (or above)

To clone it locally click the "Clone in Windows" button above or run the following git commands.

	git clone https://github.com/umco/umbraco-property-list.git umbraco-property-list
	cd umbraco-property-list
	.\build.cmd

---

## Known Issues

* _[TBC]_

---

## Contributing to this project

Anyone and everyone is welcome to contribute. Please take a moment to review the [guidelines for contributing](CONTRIBUTING.md).

* [Bug reports](CONTRIBUTING.md#bugs)
* [Feature requests](CONTRIBUTING.md#features)
* [Pull requests](CONTRIBUTING.md#pull-requests)

### TODO

What's left to do?

- [x] Pre Value Editor
	- [x] Prevalues
		- [x] DataType Picker
			- [x] Only save the ID
		- [x] Minimum items
		- [x] Maximum items
		- [x] Hide label
		- **Ideas**
			- [ ] Disable sorting?

- [ ] Value Editor
	- [x] ContentType preview
	- [x] HTML view
		- [x] Check if we can we reuse any Umbraco directives?
		- [x] Check if any UMCO projects are useful for reuse?
	- [x] CSS
	- [x] Angular / JS
		- [x] Prepare the value-editor
			- [x] Get the DataType by ID; then get...
				- [x] config/prevalues
				- [x] view-path
				- [x] property alias
			- [x] Initialize the list values
			- [x] Set the list values
			- [x] Set the IsDirty flag
		- [x] Render the DataType/property-editor
			- [x] Repeatable
			- [x] Addable
			- [x] Removeable
			- [x] Sortable
		- [x] Saving the values
			- [x] PropertyValueEditor
				- [x] ConvertDbToString
				- [x] ConvertDbToEditor
				- [x] ConvertEditorToDb
	- [x] Browser testing (Chrome, Firefox, IE/Edge)
	
- [x] PropertyValueConverter
	- [x] Get target DataType definition
	- [x] Create dummy PropertyType (in order to run the target property-editor's value-converter)
	- [x] Return as IEnumerable of that type
	- [x] Investigate ModelsBuilder support - think it's to provide the return type

- [x] Packaging
	- [x] MSBuild script
		- [x] Umbraco package
		- [x] NuGet package
	- [x] AppVeyor

- [ ] Courier data-resolver
	- [ ] Pre Value Editor
		- [ ] Add DataType dependency
	- [ ] Value Editor
		- [ ] Processing all list item DataTypes


---

## Contact

Have a question?

* [Raise an issue](https://github.com/umco/umbraco-property-list/issues) on GitHub

## Dev Team

* [Lee Kelleher](https://github.com/leekelleher)
* [Matt Brailsford](https://github.com/mattbrailsford)

## License

Copyright &copy; 2017 UMCO, Our Umbraco and [other contributors](https://github.com/umco/umbraco-property-list/graphs/contributors)

Licensed under the [MIT License](LICENSE.md)
