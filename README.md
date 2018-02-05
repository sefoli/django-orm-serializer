# django-orm-serializer
This serializer support django org data to json or xml

## Requirements

..*Python(3.4, 3.5, 3.6)
..*Django(1.10, 1.11, 2.0)

## Installation

```pip install django-orm-serializer```

## Example

```python
#get single data from django-orm
from ormserializer import Serializer
serializer = Serializer()
data = Model.objects.get(fieald=query)
result_dict = serializer.serializer_to_dict(data)
```
