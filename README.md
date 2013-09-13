### LJ Mobile Detect for Craft CMS

This is an implementation of the [Mobile Detect project](https://github.com/serbanghita/Mobile-Detect) for [Craft CMS](http://buildwithcraft.com).

**Installation**

1. Unzip file 
2. Place `lj_mobiledetect` directory into your `craft/plugins` directory
3. Install plugin in the Craft Control Panel under Settings > Plugins

**Usage**

    {{ craft.lj_mobiledetect.type }}

**Example output**

+ `tablet`
+ `phone`
+ `none`

**Example useage**

    {% if craft.lj_mobiledetect.type == "tablet" %} 
        I am a tablet
    {% elseif craft.lj_mobiledetect.type == "phone" %} 
        I am a mobile phone
    {% else %}
        I am not a mobile device
    {% endif %}

**Get `Mobile Detect` library version number**

    {{ craft.lj_mobiledetect.version }}

**Example output**

    2.6.9

**Tested on**

+ Craft 1.1