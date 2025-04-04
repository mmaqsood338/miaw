<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>MIAW Chat with Custom Styling</title>
  <meta http-equiv="Content-Security-Polic dcdy" content="script-src 'self' https://amplify--bsbox.sandbox.my.site.com">
</head>

<body>

<script type="text/javascript">
  function initEmbeddedMessaging() {
    try {
      embeddedservice_bootstrap.settings.language = 'en_US';

      window.addEventListener("onEmbeddedMessagingReady", () => {
        console.log("Inside Prechat API!!");

        embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({ "Email": "edam_system_access_user@example.com" });
        embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({ "Current_Context": "webportal" });
        embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({ "AMP_inst_id": "79886" });
        embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({ "Referral_URL": "google.com" });
        embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({ "Phone": "99897" });
        embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({ "First_Name": "Maq git" });
        embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields({ "Last_Name": "Mohammed" });
      });

      embeddedservice_bootstrap.init(
        '00DOv00000169rF',
        'MIAW_Chat_in_Amplify_Product',
        'https://amplify--bsbox.sandbox.my.site.com/ESWMIAWChatinAmplifyP1713006318201',
        {
          scrt2URL: 'https://amplify--bsbox.sandbox.my.salesforce-scrt.com'
        }
      );
    } catch (err) {
      console.error('Error loading Embedded Messaging: ', err);
    }
  }

  // Monitor DOM and apply inline styles once MIAW is injected
  const observer = new MutationObserver(() => {
    const chatButton = document.querySelector('.embedded-messaging-button');
    const chatContainer = document.querySelector('.embedded-messaging-frame-container');

    if (chatButton) {
      chatButton.style.border = '2px solid #ff6600';
      chatButton.style.borderRadius = '10px';
      chatButton.style.boxShadow = '0 2px 6px rgba(0,0,0,0.3)';
    }

    if (chatContainer) {
      chatContainer.style.border = '2px solid #ff6600';
      chatContainer.style.borderRadius = '12px';
      chatContainer.style.boxShadow = '0 8px 20px rgba(0,0,0,0.2)';
    }
  });

  observer.observe(document.body, { childList: true, subtree: true });
</script>

<!-- Load MIAW Bootstrap JS -->
<script type="text/javascript"
  src="https://amplify--bsbox.sandbox.my.site.com/ESWMIAWChatinAmplifyP1713006318201/assets/js/bootstrap.min.js"
  onload="initEmbeddedMessaging()">
</script>

</body>
</html>
