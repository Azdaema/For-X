[DEMO](https://codepen.io/Azdaema/pen/qBqRJaJ)

# Skins
Skins are CSS files you can pair with AO3 works. For more about skins, go [here](https://archiveofourown.org/admin_posts/80)

When you use a skin, AO3 provides a button, "Hide Creator's Style," which can be used to turn the skin off. (I think this exists for people with mirages or something, so sometimes find colors hard on their eyes?) This is the reason that I include the characters names with all their texts. If someone turns the skin off, the story should still be intelligible: we should still know who's talking.

# \<dl\> list
Conversations are built around the `<dl>` list, which you can learn more about [here](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dl).

# WhatsApp
For a better rundown of the features of WhatApp that this skin has, see [here](https://github.com/Azdaema/AO3-Skin_Messaging/tree/master/WhatsApp).

# Convos
For a back-and-forth convo, it'd be something like this. `out` means an outgoing message (aka one sent from the POV phone). `in` means an incoming message.

```html
<blockquote class="phone">
	<dl class="whatsapp">
		<div class="in">
			<dt>Valerio</dt>
			<dd>You ok?</dd>
		</div>
		<div class="out">
			<dt>Lu</dt>
			<dd>Yeah, fine</dd>
		</div>
	</dl>
</blockquote>
```
