Chapter code:
* [chpt12](./chpt12.html) and [chpt23](./chpt23.html) contain text messages.
* [chpt10](./chpt10.html) contains a note card.

# Structure
The outer wrapper is `<blockquote class="phone">` to distinguish it from surrounding story paragraphs.

The `notifications` are done in a [`<dl>` list](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/dl) used. In the `<dl>` list, `<dt>` is the name of person, and `<dd>` is the message itself.

Currently `notifications` is set up with 2 different types of notifications: `text` and `call`. More could be added in the future.

These can be used with different tags. If you only care about the relative time (ie. "1m ago") and not absolute time (ie. "9:37") then just use the `<div>` tag:

```html
<blockquote class="phone">
	<dl class="notifications">
		<div class="text">
			<dt>Jaime Lannister <span class="time">now</span> </dt>
			<dd>I'm outside. We can still run.</dd>
		</div>
	</dl>
</blockquote>
```

If you want to be able to hover over a notification and see the absolute time it was sent, use `<dfn>` like this:

```html
<blockquote class="phone">
	<dl class="notifications">
		<dfn class="text" title="19:35">
			<dt>Jaime Lannister <span class="time">now</span> </dt>
			<dd>I'm outside. We can still run.</dd>
		</dfn>
	</dl>
</blockquote>
```

`<dfn>` doesn't show up on mobile. On a phone, both of the two would function the same.

## Hide Creator's Style
If a reader clicks "Hide Creator's Style" then it would look like this:
<blockquote class="phone">
	<dl class="notifications">
		<div class="text">
			<dt>Jaime Lannister <span class="time">now</span> </dt>
			<dd>I'm outside. We can still run.</dd>
		</div>
	</dl>
</blockquote>
