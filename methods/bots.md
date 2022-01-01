# Bots

{% swagger baseUrl="https://api.atlasbots.com" path="/bot/:botID" method="get" summary="Bots" %}
{% swagger-description %}

{% endswagger-description %}

{% swagger-parameter in="path" name="id" type="string" required="true" %}
ID of the bot you would like the information about.
{% endswagger-parameter %}

{% swagger-response status="200" description="Bots information send successfully." %}
```
This content of this response varies.
```
{% endswagger-response %}

{% swagger-response status="404" description="Unable to find the bot on our system." %}
```
{    "message": "[Atlas API] Bot not found. Please provide a valid Bot ID. Should be a String or Discord Snowflake"}
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

{% swagger-response status="200" description="Bots stats posted successfully" %}
```
{ "message": "[Atlas API] Your Stats have been posted! Now go enjoy your day Noob!"}
```
{% endswagger-response %}

{% swagger-response status="400: Bad Request" description="Bad Request from server." %}
```javascript
This content of this response varies.
```
{% endswagger-response %}

{% swagger-response status="404" description="Unable to find the bot on our system." %}
```
{    "message": "[Atlas API] Bot not found. Please provide a valid Bot ID. Should be a String or Discord Snowflake"}
```
{% endswagger-response %}
{% endswagger %}
