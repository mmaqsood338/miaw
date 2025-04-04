<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>MIAW Chat with Custom Styling</title>

  <!-- Custom CSS Styling -->
  <style>
    /* Style the chat launcher button */
    .embedded-messaging-button {
      border: 2px solid #ff6600 !important;
      border-radius: 10px !important;
      box-shadow: 0 2px 6px rgba(0, 0, 0, 0.3) !important;
    }

    /* Style the full chat window container */
    .embedded-messaging-frame-container {
      border: 2px solid #ff6600 !important;
      border-radius: 12px !important;
      box-shadow: 0 8px 20px rgba(0, 0, 0, 0.2) !important;
      overflow: hidden !important;
    }
  </style>
</head>

<body>
  <!-- Salesforce Embedded Messaging -->
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
  </script>

  <!-- Load MIAW JS Bootstrap -->
  <script type="text/javascript"
    src="https://amplify--bsbox.sandbox.my.site.com/ESWMIAWChatinAmplifyP1713006318201/assets/js/bootstrap.min.js"
    onload="initEmbeddedMessaging()"></script>
</body>
</html>
