---
layout: default
title: Security Test
---

## XSS Test Page

{% raw %}
{% highlight javascript %}
// Test 1
console.log("URL: " + window.location.href);

// Test 2
function testAlert() {
    alert("Domain: " + document.domain);
}
testAlert();
{% endhighlight %}
{% endraw %}

## Test Section

```javascript
// Additional test
document.addEventListener('DOMContentLoaded', () => {
    console.log("Page loaded");
});
```
