# Bots

{% swagger baseUrl="https://api.atlasbots.com" path="/bot/:botID" method="get" summary="Bots" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="id" type="string" required="true" %}
ID of the bot you would like the information about.
{% endswagger-parameter %}

{% swagger-response status="200" description="Cake successfully retrieved." %}
```
{    "name": "Cake's name",    "recipe": "Cake's recipe name",    "cake": "Binary cake"}
```
{% endswagger-response %}

{% swagger-response status="404" description="Could not find a cake matching this query." %}
```
{    "message": "Ain't no cake like that."}
```
{% endswagger-response %}
{% endswagger %}



{% swagger baseUrl="https://api.atlasbots.com" path="/stats/:botID" method="get" summary="Post Stats" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="id" type="string" required="true" %}
ID of the bot you would like to post stats to.
{% endswagger-parameter %}

{% swagger-parameter in="header" name="Authentication" type="string" required="true" %}
The bot's Authentication token 
{% endswagger-parameter %}

{% swagger-response status="200" description="Cake successfully retrieved." %}
```
{    "name": "Cake's name",    "recipe": "Cake's recipe name",    "cake": "Binary cake"}
```
{% endswagger-response %}

{% swagger-response status="404" description="Could not find a cake matching this query." %}
```
{    "message": "Ain't no cake like that."}
```
{% endswagger-response %}
{% endswagger %}
