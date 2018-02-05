# django-orm-serializer
This serializer support django org data to json or xml

## Requirements

* Python(3.4, 3.5, 3.6)
* Django(1.10, 1.11, 2.0)

## Installation

```pip install django-orm-serializer```

## Example

* Get single data from django-orm. `serialize_to_dict` This funtion has attributes which help returning data quality. 

| Option    | Help                                      |
|-----------|-------------------------------------------|
| instance  | Django query object                       |
| cur_dept  | Starting dept value default=1             |
| max_dept  | Maximum dept value default=2              |

```python
from ormserializer import Serializer
serializer = Serializer()
data = Model.objects.get(fieald=query)
result_dict = serializer.serializer_to_dict(data)
```
