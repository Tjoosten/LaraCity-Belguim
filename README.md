# LaraCity Belguim
Migration and seed files with all all the cities of Belguim for Laravel PHP Framework.

## A Simple Example of Use
#### Controller
```php
	/**
	* Show the form for creating a new resource.
	*
	* @return View
	*/
	public function create()
	{
		$countries = Cities::all();

		return View::make('myview', compact('cities'));
	}
```
#### View
```html
    <select class="form-control" name="country">
        <option value="">Select a city</option>
        @foreach($cities as $city)
            <option value="{{ $city->id }}">{{ $city->Gemeente }}</option>
        @endforeach
    </select>
```

## License
Copyright (c) 2015 [Tim Joosten](http://www.rientjeteen.be). See the LICENSE
file for license rights and limitations (MIT).
