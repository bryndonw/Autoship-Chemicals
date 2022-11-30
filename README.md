# Autoship-Chemicals
Ok so here we go!
This is an example of the code for the buttons. 
Follow [these instructions](https://developer.paypal.com/api/nvp-soap/paypal-payments-standard/integration-guide/subscribe-step-1/) and you should be able to get the code that will look similar to this:
```
<div id="paypal-button-container3">
<script>
  paypal.Buttons({
      style: {
          shape: 'pill',
          color: 'blue',
          layout: 'vertical',
          label: 'subscribe'
      },
      createSubscription: function(data, actions) {
        return actions.subscription.create({
          'plan_id': 'P-5LV1202761046713KL73TQJY'
        });
      },
      onApprove: function(data, actions) {
        alert(data.subscriptionID);
      }
  }).render('#paypal-button-container3');
</script>
</div>
    

 </div>
```

You will probably have to update code for all of the buttons (3 buttons for each product). 
The code for all of the buttons is located in General Blocks in WordPress. 
There are 4 blocks, all labeled Autoship Chemicals # (example Autoship 1).
The code will be located in the custom html section.
