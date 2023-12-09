<html>
	<body>
		<script type='text/javascript'>
	function initEmbeddedMessaging() {
		try {
			embeddedservice_bootstrap.settings.language = 'en_US'; // For example, enter 'en' or 'en-US'
			window.addEventListener("onEmbeddedMessagingReady", () => {            
	console.log( "Inside Prechat API!!" );
	embeddedservice_bootstrap.prechatAPI.setHiddenPrechatFields( { "Hiddenemail" : "mmohammed@amplify.com" } );
});
			embeddedservice_bootstrap.init(
				console.log( "Inside INIT!" );
				'00DNq000000H9QH',
				'Miaw_git_hub',
				'https://amplify--sandboxpc.sandbox.my.site.com/ESWMiawgithub1702107659319',
				{
					console.log( "Inside scrt!" );
					scrt2URL: 'https://amplify--sandboxpc.sandbox.my.salesforce-scrt.com'
				}
			);
		} catch (err) {
			console.error('Error loading Embedded Messaging: ', err);
		}
	};
</script>
<script type='text/javascript' src='https://amplify--sandboxpc.sandbox.my.site.com/ESWMiawgithub1702107659319/assets/js/bootstrap.min.js' onload='initEmbeddedMessaging()'></script>


	</body>
</html>
