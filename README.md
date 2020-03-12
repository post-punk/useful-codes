Remove object with a certain property from the array:
```
var rockets = [
    { country:'Russia', launches:32 },
    { country:'US', launches:23 },
    { country:'China', launches:16 },
    { country:'Europe(ESA)', launches:7 },
    { country:'India', launches:4 },
    { country:'Japan', launches:3 }
];

//find its index first
var badElement = rockets.findIndex(el=> {
	return el.country.includes('US');
});

//splice that shit
rockets.splice(badElement, 1);
```
