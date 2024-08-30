BASE.html
```html
<title>
      {% block title %} The Panipat Handloom | One Stop Shop to all your interior needs{% endblock %}
</title>

```

Category

```html

{% block title %}
    {% if sub_cat.meta_title %}
        {{ sub_cat.meta_title }}
    {% else %}
        Shop the {{ sub_cat.sub_cat_title }} at The Panipat Handloom Emporium | One Stop Solution for all your Interior Needs
    {% endif %}
{% endblock %}

{% block meta %}
   <meta name="description" content="{{sub_cat.description}}">
   <link rel="canonical" href="{{sub_cat.canonical_link}}" />
   <meta name="robots" content="{% if sub_cat.meta_robots == "1" %}noindex,nofollow,all{% else %}{{sub_cat.meta_robots}}{% endif %}" />
   <meta name="author" content="The Panipat Handloom Emporium" />
   <meta name="copyright" content="The Panipat Handloom Emporium" />
   <!--  og tags -->
   <meta property="og:type" content="website" />
   <meta property="og:url" content="{{sub_cat.og_url}}" />
   <meta property="og:site_name" content="The Panipat Handloom Emporium" />
   <meta property="og:locale" content="en_US" />
   <meta property="og:title" content="{{sub_cat.og_title}}" />
   <meta property="og:description" content="{{sub_cat.og_description}}" />

   <meta property="og:image" content="{% if sub_cat.og_image == "1" %}https://thepanipathandloom.com/static/wp-content/themes/minimog/assets/images/final-banner1.jpg{% else %}{{ sub_cat.og_image }}{% endif %}" />

   <meta property="og:image:type" content="image/jpeg" />
   <meta property="og:image:width" content="1200" />
   <meta property="og:image:height" content="630" />
   <meta name="twitter:card" content="summary_large_image" />
   <meta name="twitter:site" content="The Panipat Handloom - One Stop Solution for all your interior needs" />
   <meta name="twitter:creator" content="@HandloomPanipat" />
   <meta name="twitter:url" content="https://x.com/HandloomPanipat">
   <meta name="twitter:title" content="{{sub_cat.twitter_title}}">
   <meta name="twitter:description" content="{{sub_cat.twitter_description}}." />
   <meta property="twitter:image" content="https://thepanipathandloom.com/static/assets/website-2.jpg" />
   <meta property="twitter:image:type" content="image/jpeg" />
   <meta property="twitter:image:width" content="1200" />
   <meta property="twitter:image:height" content="630" />
   
   <meta name="mobile-web-app-capable" content="yes" />
   <meta name="apple-mobile-web-app-capable" content="yes" />
{% endblock %}

```






new meta | base
```
{% block meta %}
    <meta name="description" content="Enhance Your Interior with The Panipat Handloom - one stop solution for all your interior needs in Delhi! Our expert interior solutions ensure peace of mind. Contact us today for top-notch interiors and designs">
    <meta name="keywords" content="">
    <link rel="canonical" href="https://thepanipathandloom.com/" />
    <meta name="robots" content="index,follow,all" />
    <meta name="author" content="The Panipat Handloom Emporium" />
    <meta name="copyright" content="The Panipat Handloom Emporium" />
    <!--  og tags -->
    <meta property="og:type" content="website" />
    <meta property="og:url" content="thepanipathandloom.com/" />
    <meta property="og:site_name" content="The Panipat Handloom Emporium" />
    <meta property="og:locale" content="en_US" />
    <meta property="og:title" content="The Panipat Handloom Emporium in Delhi" />
    <meta property="og:description" content="Enhance Your Interior with The Panipat Handloom - one stop solution for all your interior needs in Delhi! Our expert interior solutions ensure peace of mind. Contact us today for top-notch interiors and designs." />
    <meta property="og:image" content="https://thepanipathandloom.com/static/assets/website-2.jpg" />
    <meta property="og:image:type" content="image/jpeg" />
    <meta property="og:image:width" content="1200" />
    <meta property="og:image:height" content="630" />
    <meta name="twitter:card" content="summary_large_image" />
    <meta name="twitter:site" content="The Panipat Handloom - One Stop Solution for all your interior needs" />
    <meta name="twitter:creator" content="@HandloomPanipat" />
    <meta name="twitter:url" content="https://x.com/HandloomPanipat">
    <meta name="twitter:title" content="">
    <meta name="twitter:description" content="Enhance Your Interior with The Panipat Handloom - one stop solution for all your interior needs in Delhi! Our expert interior solutions ensure peace of mind. Contact us today for top-notch interiors and designs." />
    <meta property="twitter:image" content="https://thepanipathandloom.com/static/assets/website-2.jpg" />
    <meta property="twitter:image:type" content="image/jpeg" />
    <meta property="twitter:image:width" content="1200" />
    <meta property="twitter:image:height" content="630" />

    <meta name="mobile-web-app-capable" content="yes" />
    <meta name="apple-mobile-web-app-capable" content="yes" />
    {% endblock %}

```
