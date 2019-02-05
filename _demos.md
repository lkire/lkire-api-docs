# Demos

## Get All Demos

```python
import lkire-api

api = lkire-api.authorize('youraccesstoken')
api.demos.get()
```

```javascript
const lkire-api = require('lkire-api');

let api = lkire-api.authorize('youraccesstoken');
let demos = lkire-api.demos.get();
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "category": "stat",
    "title": "Wavelet Time Series Analysis",
    "frame": "http://api.lkire.com/wavelet",
    "description": "Wavelets provide a complete orthonormal 
    decomposition of a function with both..."
  },
  {
    "id": 2,
    "category": "ml",
    "title": "Convolutional Neural Network Playground",
    "frame": "http://api.lkire.com/cnn",
    "description": "Convolutional neural networks embed layers 
    for the discovery of convolutionally tiled feature sets..."
  }
]
```

This endpoint retrieves all demos with your level of authentication.

### HTTP Request

`GET http://api.lkire.com/cnn`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
category | all | May be set to a category in the set {ml, phys, stat} to limit topic. 

<aside class="success">
Remember — some demos may not be visible without authentication!
</aside>