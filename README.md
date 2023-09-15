# oppe-for-python
An API wrapper for [Oppe](https://oppe.app) written in Python.


## Installation

```bash
pip install oppe
```

## Usage

### Sending an event

```python
from oppe import Oppe

oppe = Oppe(api_token='insert-api-token-here', project_id="uuid-of-project")

oppe.event(
    channel_id="uuid-of-channel",
    title="user-registered",
    description="A new user has registered.",
    emoji="👋",
    data={
        "user_id": 123,
    },
)
```
