# myDeckWishlist
<img class="size-medium wp-image-548 alignleft"  style="text-align:left;" src="https://miriamxyra.files.wordpress.com/2016/04/mx_offtopic_border.png?w=300" alt="mx_offtopic_border" width="300" height="256" />

Magic the Gathering, played with real cards, can be a very expensive hobby: If you want to buy cards for a new deck, you often have to wait some months to get all cards you need.

If you already own other cards which fit in your deck, you may also want to play them instead until you can afford the more expensive cards.

The last deck I was excited about was Bant Spirits. A great modern deck which is quite fast but has also some control elements in it.

I already owned some cards but so many were missing to finally play it.

So I began to create a list: which cards I own, how many are still missing and how much I have to pay for them...

But getting the price for every card was quite annoying: Querying <a href="http://magickartenmarkt.de">magickartenmarkt.de</a> just to find out an actual price for a card and typing it into the sheet.

So I started to create a Macro to accomplish this annoying task automatically. I think this Excel sheet became quite useful. That's why I want to share it with you.
<h1>myDeckWishlist</h1>
<em>myDeckWishlist</em> helps you to keep your missing cards tracked.
<h2>Download</h2>
You can get it here: <a href="https://github.com/miriamxyra/myDeckWishlist">https://github.com/miriamxyra/myDeckWishlist</a>
<h2>Enable Macros for this document</h2>
Since myDeckWishlist is macro based, you have to enable macros before you can use it.

<img class="alignnone size-medium wp-image-841" src="https://miriamxyra.files.wordpress.com/2017/01/macro.png?w=300" alt="macro" width="300" height="69" />

Be careful when enabling macros in documents from the internet! Only do this if you trust the source. If you are able to read programming languages always check the code before enabling macros.
<h2>The Excel sheets in myDeckWishlist</h2>
The Excel sheet has two sheets: <em>Deck List</em> and <em>Cost Overview</em>. You only enter data in the <em>Deck List</em> sheet. <em>Cost Overview</em> is generated automatically.
<h3>Deck List</h3>
<img class="alignnone wp-image-840 size-full" src="https://miriamxyra.files.wordpress.com/2017/01/mydeckwishlist.png" alt="mydeckwishlist"  />

You have to fill out four columns for each card:
<ul>
 	<li><em><strong>No#</strong></em>: how many cards will be needed in this Deck</li>
 	<li><em><strong>Name</strong></em>: what's the name of the card</li>
 	<li><em><strong>Type</strong></em>: what kind of type is this card (the type is needed for the Cost Overview pivot table)</li>
 	<li><em><strong>How many I already got</strong></em>: speaks for itself, I suppose...</li>
</ul>
<img class="alignnone wp-image-851" src="https://miriamxyra.files.wordpress.com/2017/01/columns.png" alt="columns" width="489" height="227" />

On the right side you can choose if you want to query the prices for your mainboard or sideboard only - or for both.

<img class="alignnone wp-image-852" src="https://miriamxyra.files.wordpress.com/2017/01/gatherprices.png" alt="gatherprices" width="415" height="308" />

When you click on "Calculate MKM prices" the prices for the table(s) of your choice will be queried and the table(s) will be filled out with the <strong>minimum price</strong> for each card.

This process takes a bit time because it queries the MKM for every card to get the actual prices.

While the prices are being fetched you see in the bottom left corner which card is queried.

<img class="alignnone size-medium wp-image-854" src="https://miriamxyra.files.wordpress.com/2017/01/queryingmkm1.png?w=300" alt="queryingmkm" width="300" height="54" />

When all prices are fetched the Application bar shows the status "ready".

<img class="alignnone size-medium wp-image-855" src="https://miriamxyra.files.wordpress.com/2017/01/queryingmkm_ready.png?w=300" alt="queryingmkm_ready" width="300" height="54" />
<h3>Cost Overview</h3>
In the cost overview sheet you can easily see where the most expensive card types are.

<img class="wp-image-867 size-large aligncenter" src="https://miriamxyra.files.wordpress.com/2017/01/pivot.png?w=620" alt="pivot" width="620" height="147" />Maybe you can already play your deck if you only exchange your manabase..?

<img class="wp-image-856 size-large aligncenter" src="https://miriamxyra.files.wordpress.com/2017/01/pivot_expand.png?w=620" alt="pivot_expand" width="620" height="628" />

When you query MKM market with the button on the <em>Deck List</em> page, these pivot tables will be refreshed automatically. If you make other changes without querying prices, you can refresh them with the <em>Refresh Pivot Tables</em> Button, too.
<h1>Donate and Share</h1>
If you like myDeckWishlist and you want to support me, feel free to donate here: <a href="https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=miriamxyra%40gmail%2ecom&lc=GB&item_name=miriamxyra&no_note=0&currency_code=EUR&bn=PP%2dDonationsBF%3abtn_donate_LG%2egif%3aNonHostedGuest">Donate</a>

You may also share it with your friends and comment <a href="http://wp.me/p5QwIJ-dj">miriamxyra.com</a>. It's not perfect yet, so if you have any suggestions for improvement, let me know.
