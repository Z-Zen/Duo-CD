# Duo-CD
Duo calculator for Crimson Desert created with Claude Code (Opus 4.6).

# How it works

The Duo deck has 20 cards (Red and Yellow 1-10). You know your 2 cards, and you can see 1 card from each opponent. The calculator takes all the cards you can't see and checks every single possible way those hidden cards could be distributed among your opponents.

So, the number of possible hidden card combinations is small enough to check them all. The calculator literally plays out every possible deal and counts wins vs losses.

`Win % = (scenarios you win) / (total possible scenarios)`

For example, say you have 7 Points and Opponent A shows a Red 4. The calculator goes through every card that could be their hidden second card,  but it doesn't stop there. If Opponent B is also at the table, it makes sure the card it "gave" to A isn't also given to B. It checks all valid combinations at once, not one opponent at a time.

For each possible deal, it plays out the matchup using the full hand ranking rules (Prime Pair, Superior Pair, Judge, Warden, etc.) and counts how many of those scenarios you win. Your win % is just: scenarios you win / total possible scenarios.

Cheat Mode does the same thing, but in reverse. When you're dealing, you can peek at your opponent's cards. You input both of each opponent's cards, and it tells you which card to pick by averaging your win rate across every possible random second card you could be dealt.

Hidden Card (Stash) lets you simulate the in-game card hiding mechanic. While dealing, you can secretly pocket one card from the deck. That card stays with you across rounds. During any opponent's "thinking" phase, a "Change Hand" window appears — that's when you can swap your stashed card into your hand. The swap is bidirectional: the card you replace becomes your new stash.

The Swap Advisor shows all 3 options (keep hand, swap with card 1, swap with card 2) with exact win % for each, so you  know exactly when to pull the trigger. The idea is to hold a strong card until the AI bets big, then swap it in, go all-in, and leave the table.
