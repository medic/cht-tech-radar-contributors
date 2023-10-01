---
title:      "WebDriverIO"
ring:       adopt
quadrant:   languages-and-frameworks
tags:       [quality]
---

[WebDriverIO](https://webdriver.io/) is UI testing framework used for end-to-end testing in web applications.

In the CHT Core Framework, WebDriverIO is used to [run the e2e tests](https://github.com/medic/cht-core/tree/master/tests/e2e).

WebDriverIO was influenced by a lot of Protractor's design decisions which is why it was the closest framework to migrate over.

### Advantages
* Open source
* Numerous integrations to tools
* Fast and easy location of page elements
* Good documentation

### Drawbacks
* Integrations with reports (specifically allure) frameworks is not straightforward.

The migration from Protractor was finalized in July 2023. 