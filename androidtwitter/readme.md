This example comes from Libby Baldwin at
http://www.mobiledevelopersolutions.com/home/start/twominutetutorials/tmt5p1
https://github.com/libbybaldwin/applaud-tmt5p1-oauth-twitter

My addition was a button to clear the local cache so you can practice logins with 
multiple Twitter accounts:

	<!-- Burr -->
	<div id="clearCache">
		<div data-role="button" id="clearButton">Clear Cached Creds</div>
	</div>

and

    $('#clearCache').click(function() {
    	localStorage.removeItem(localStoreKey);
    	alert(localStoreKey + " removed");
    });


You will need to edit main.js to inject your keys

            consumerKey: 'fromTwitter',
            consumerSecret: 'fromTwitter',

And you should have your own public URL that serves as the redirect point.  You
can search for instances of "burrsutter" for areas that need replacement with your URLs