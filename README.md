# vs-code-snippets
A collection of all snippets/boiler-plate usable in VS code (Currently working on Python snippets)

## Table of Contents
- [Python](#python)
- [Julia](#julia)

---

## Python

| Prefix              |           Description                      |
| ------------------- | -------------------------------------------|
| propertygetter      | Python [property](#propertygetter) getter |
| propertysetter      | Python [property](#propertysetter) getter and setter |
| classinit           | Python [class](#classinit) with an `__init__()`  |
| classreprstr        | Python [class](#classreprstr) with `__str__()` and ` __repr__()` |
| classsequence       | Python [class](#classsequence) with `__init__()`, `__getitem__()`, `__setitem__()`, `__delitem__()`, `__len__()`, and `insert()` |

## Julia
TODO

---

# Code Reference

## Python

##### `propertygetter`

```python
@property
def name(self):
    return self._name
```

##### `propertysetter`
```python
@property
def name(self):
    return self._name

@name.setter
def name(self, ):
    self._name = 
```

##### `classinit`
```python
class Name(object):

    def __init__(self):
        pass

```

##### `classreprstr`
```python
class Name(object):

    def __repr__(self):
        """Representation of repr()."""
        pass

    def __str__(self):
        """Representation of str()."""
        pass
```

##### `classsequence`
```python
class Name(object):

    def __init__(self):
        self._data = dict()

    def __getitem__(self, key):
        """Getter."""
        value = self._data[key]
        return value

    def __setitem__(self, key, value):
        """Setter."""
        self._data[key] = value

    def __delitem__(self, key):
        """Delete Key"""
        del self._data[key]

    def __len__(self):
        """Length"""
        return len(self._data)

    def insert(self):
        pass

```

# Contribution
Create a new branch and start a pull request.
