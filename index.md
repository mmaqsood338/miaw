<html>

	<meta http-equiv="Content-Security-Policy" content="default-src 'self'; frame-src 'self' *.salesforce.com *.force.com;">


	<body>
		<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'

			embeddedservice_bootstrap.init(
				'00DNq000000H9QH',
				'Web_Chat',
				'https://amplify--sandboxpc.sandbox.my.site.com/ESWWebChat1700673748355',
				{
					scrt2URL: 'https://amplify--sandboxpc.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://amplify--sandboxpc.sandbox.my.site.com/ESWWebChat1700673748355/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>

	</body>
</html>
