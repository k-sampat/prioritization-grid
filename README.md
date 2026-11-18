# prioritization-grid

A page for putting a list in order by comparing two items at a time, using the Prioritizing Grid method from *What Color Is Your Parachute?*

> Built for my own use and tested in Chrome on macOS.

## How to use it

1. Download `index.html` and open it in your browser. It loads its styles from the internet, so it needs a connection.
2. Paste your list, one item per line or all on one line separated by commas. Numbers and bullets at the start of a line get taken out, and an item that appears twice is kept once.
3. Pick between two items at a time. Click one, or press ← or 1 for the left item and → or 2 for the right one. Backspace goes back a pair.
4. When every pair is done, you get the list in order, with how many times you picked each item. "Copy the list" puts it on your clipboard.
5. "Start over" clears the list when you've finished with it.

Every pair gets compared once, so 10 items is 45 pairs and 20 items is 190. The page saves your picks as you go, so you can stop and come back.

You can change the question asked at each pair. The default is "Which matters more to you?", and for a list of things you want to avoid, "Which do I dislike more?" works better.

## The grid

The pairs come in the same order as the book's grid: 1 and 2, then 2 and 3, and on down the diagonal. That way the same item doesn't come up many times in a row.

Under the pair on screen is the grid itself, with one box for every pair and the number you picked filled in. Click any box to go back to that pair and change your pick.

## Ties

| Tied items | What happens |
|---|---|
| Two | The one you picked when you compared those two goes higher. This is the book's rule. |
| Three or more | The book says to put them in order by gut. This page starts from your own picks among those items, and the one you picked most often among them goes higher. Any that are still tied go through the same steps again. |
| A circle | If you picked A over B, B over C and C over A, none of them wins head-to-head, so the page asks you to change one of those picks. |

Breaking a tie only reorders items with the same count. An item never moves above one you picked more often.

Every tie has a "Compare these again" link, which shows just the pairs among the tied items with the picks you made. Leave them as they are, or change any you see differently now. A change there only reorders the tied items, and the grid and the counts stay as they were. To change a pick everywhere, counts included, click its box in the grid.

## Where your picks are kept

In your browser's own storage, on your computer. Nothing is sent anywhere.

The page holds one list at a time and saves it after every pick, so reloading or closing the tab doesn't lose your place. "Start over" deletes the list from the browser. A different browser starts empty. So does clearing your browser's site data.

## Colors

The menu in the header has 13 light themes and 8 dark ones, and the button next to it switches between light and dark. The page remembers what you chose.

## Credits

The method is Richard N. Bolles' Prioritizing Grid, from *What Color Is Your Parachute?* Nothing from the book is copied here, and the tie rules above are in my own words.

The styles and themes are [daisyUI](https://daisyui.com) 5.7.50 by Pouya Saadeghi, under the MIT license, loaded from [jsDelivr](https://www.jsdelivr.com).

## License

MIT. See [LICENSE](LICENSE).
