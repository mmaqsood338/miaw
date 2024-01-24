<html>
<head>
	<meta Content-Security-Policy: script-src 'self' https://amplify--sandboxpc.sandbox.my.site.com>
</head>

	<body>
<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			
			window.addEventListener("onEmbeddedMessagingReady", () => {            
	console.log( "Inside Prechat API!!" );
	embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( { "Email" : "edam_system_access_user@example.com" } );
	embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( { "Current_Context" : "webportal" } );
	embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( { "AMP_inst_id" : "79886" } );
	embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( { "Referral_URL" : "google.com" } );
});

			embeddedservice_bootstrap.init(
				'00DNq000000H9QH',
				'MIAW_SF_Test',
				'https://amplify--sandboxpc.sandbox.my.site.com/ESWMIAWSFTest1702218452582',
				{
					scrt2URL: 'https://amplify--sandboxpc.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://amplify--sandboxpc.sandbox.my.site.com/ESWMIAWSFTest1702218452582/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

	</body>
</html>
