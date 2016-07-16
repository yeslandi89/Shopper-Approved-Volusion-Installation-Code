# Shopper-Approved-Volusion-Installation-Code
Shopper Approved installation code for Volusion



## Merchant Review Only

```js
<!--Shopper Approved Merchant Review Code-->
<script type="text/javascript">
    var sa_values = {"site": '<YOUR_SITE_ID>'};
    function saLoadScript(src) {
        var js = window.document.createElement("script");
        js.src = src;
        js.type = "text/javascript";
        document.getElementsByTagName("head")[0].appendChild(js);
    }
    var d = new Date();
    if (d.getTime() - 172800000 > 1468677082000)
        saLoadScript("//www.shopperapproved.com/thankyou/rate/"+sa_values.site+".js");
    else
        saLoadScript("//direct.shopperapproved.com/thankyou/rate/"+sa_values.site+".js?d=" + d.getTime());
</script>
<!--Shopper Approved Merchant Review Code-->
```
## Merchant and Proucts Reviews
```js
<!--Shopper Approved Merchant & Product Review Code-->
<script type="text/javascript">
    var sa_values = {'site': '<YOUR_SITE_ID>', 'gts': 1, 'forcecomments': 1};
    var sa_products = {};
    for (var i = 0; i < OrderDetails.length; i++) {
        sa_products[OrderDetails[i][2]] = OrderDetails[i][3];
    }
    function saLoadScript(src) {
        var js = window.document.createElement("script");
        js.src = src;
        js.type = "text/javascript";
        document.getElementsByTagName("head")[0].appendChild(js);
    }
    var d = new Date();
    if (d.getTime() - 172800000 > 1460567935000)
        saLoadScript("//www.shopperapproved.com/thankyou/rate/"+sa_values.site+".js");
    else
        saLoadScript("//direct.shopperapproved.com/thankyou/rate/"+sa_values.site+".js?d=" + d.getTime());
</script>
<!--Shopper Approved Merchant & Product Review Code-->
```

