---
title: REST API  Testing
date: 2020-11-19
tags: [api-testing,python,testing,test-automation,test-scripts,gists]
description: REST API Test using Python Request Library & Unittest 
draft: false
---

### Example:API testing Using Selenium

{{<gist jaymutuku 499235d0f098dcc97451e9637e7a9080 >}}


### Notes
[Here](https://github.com/jaymutuku/python-api-tests) is the detailed explanation of above script.

### Bonus
Below test script demos the simplest api test using python `unittest` and `request` libraries.

```python

import unittest
import requests
 
class APITest(unittest.TestCase):
	def setUp(self):
		self.base_url = "http://localhost:3000"
 
	def some_test(self):
		response = requests.get(self.base_url)
		self.assertEqual(response.json(), {"result": 30})
 
if __name__ == "__main__":
	unittest.main()


```

### TODO:
For Above Script,implement a simple web api service that returns the result as shown in the script.


