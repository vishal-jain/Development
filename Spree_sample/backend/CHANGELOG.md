## Spree 2.2.0 (unreleased) ##

* Don't serve JS to non XHR requests. Prevents sentive data leaking. Thanks to
  Egor Homakov for pointing that out in Spree codebase.
  See http://homakov.blogspot.com.br/2013/05/do-not-use-rjs-like-techniques.html
  for details.

* 'Only show completed orders' checkbox status will now persist when paging through orders.

    * darbs + Ryan Bigg

* Implemented a basic Risk Assessment feature in Spree Backend. Viewing any Order's edit page now shows the following, with a status indicator:

        Payments; link_to new log feature (ie. Number of multiple failed authorization requests)
        AVS response (ie. Billing address not matching credit card)
        CVV response (ie. code not matching)

    * Ben Radler (aka lordnibbler)
