# Shopper-Approved-Volusion-Installation-Code
Shopper Approved installation code for Volusion



## Merchant Review Only

1. Go to Volusion backend 
2. Go to `Design > Site Content`
3. Open `Article ID 130`
4. Copy and paste the code below 
5. Replace `<YOUR_SITE_ID>` with your Shopper Approved Site ID
6. Place a test order to make sure the code it's working

```js
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
```

## Merchant and Proucts Reviews

1. Go to Volusion backend 
2. Go to `Design > Site Content`
3. Open `Article ID 130`
4. Copy and paste the code below 
5. Replace `<YOUR_SITE_ID>` with your Shopper Approved Site ID
6. Place a test order to make sure the code it's working



```js
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
```

