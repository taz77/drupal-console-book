# config:export
वर्तमान अनुप्रयोग कॉन्फिगरेशन निर्यात करा.

**Usage:**
```
drupal config:export [options]
ce
```

## Available options
Option | Details
-------|-------------
--directory | कॉन्फिगरेशन आऊटपुट जतन करण्यासाठी निर्यात डिरेक्ट्रीची व्याख्या करा.
--tar | सेट केल्यास, कॉन्फिगरेशनला संग्रहण फाईलवर निर्यात केले जाईल.
--remove-uuid | सेट केल्यास, uuid कीशिवाय कॉन्फिगरेशन निर्यात केले जाईल.
--remove-config-hash | सेट केल्यास, डीफॉल्ट साइट हॅश कीशिवाय कॉन्फिगरेशन निर्यात केले जाईल.

## Examples
* पर्यायी आपण निर्यात करण्यासाठी मार्ग जोडू शकता
```
drupal config:export  \
  --directory="path/to/export"
```
* जर निर्यात संकुचित फाइलमध्ये असेल आणि / किंवा जर uuid आणि कॉन्फिग हॅश काढून टाकले जातील.
```
drupal config:export  \
  --directory="path/to/export" \
  --tar \
  --remove-uuid \
  --remove-config-hash
```
