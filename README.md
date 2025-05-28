# ifream-tracking-for-same-domain

i frame hidden domain Code:

<script>
(function(){
  // only run inside the iframe domain
  if(location.hostname !== 'embed.perfectvenue.com') return;

  // wrap the dataLayer.push method
  var origPush = dataLayer.push;
  dataLayer.push = function(obj) {
    origPush.call(dataLayer, obj);
    if(obj.event === 'Form Submitted Complete') {
      parent.postMessage(
        { event: 'form_submit_iframe', formData: obj },
        'https://www.harringtonssf.com'
      );
    }
  };
})();
</script>



Triggerr: Page Hostname > equals > iframe Doamin


Main Domain Code:


<script>
window.addEventListener('message', function(e) {
  if(e.origin !== 'https://embed.perfectvenue.com') return;
  dataLayer.push(e.data);
});
</script>



Triggerr: All Page
