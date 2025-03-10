---
layout: default
title: Security Test Page
---

# XSS POC Demo

## Test Cases

### 1. Basic XSS Test
{% raw %}
{% highlight javascript %}
// Basic console output
console.log("Page loaded successfully");
{% endhighlight %}
{% endraw %}

### 2. Theme Processing Test
```javascript
// Theme customization test
document.addEventListener('DOMContentLoaded', () => {
    console.log("Theme loaded");
});
```

### 3. Markdown Processing Test
[Click me](javascript:alert('Markdown XSS Test'))

### 4. HTML Injection Test
<div id="test">
Testing HTML processing
</div>

### 5. Plugin Test
{% raw %}
{% highlight python %}
def test():
    print("Plugin test")
{% endhighlight %}
{% endraw %}

## Results
Check the browser console and alerts for test results.
