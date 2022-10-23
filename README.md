# MediaWiki skin for Eithalica Wiki

This skin requires you to specify either dark mode or light mode, by applying the `dark-mode` or `light-mode` class to the `body` element. To do this, add the following code to your `LocalSettings.php` file:

	# Courtesy of Samwilson from MediaWiki: https://www.mediawiki.org/w/index.php?title=Topic:V2tzn1fwy6lwa6m6&topic_showPostId=v2ulvjo1d1v4h608#flow-post-v2ulvjo1d1v4h608
	$wgHooks['OutputPageBodyAttributes'][] = function ( OutputPage $out, Skin $skin, &$bodyAttrs ) {
	  $bodyAttrs['class'] .= ' dark-mode'; // Note the leading space character.
	};

(If you want light mode, replace `dark-mode` in the above code with `light-mode`.)

