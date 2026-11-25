# Poker Showdown Evaluator: Flush vs Full House

An open-source Texas Hold'em showdown referee and hand ranking comparator to settle table disputes when a Flush meets a Full House.

Live official interactive showdown calculator: [flush vs full house who wins](https://flopkit.com/who-wins/flush-vs-full-house/) on [FlopKit](https://flopkit.com/).

---

## The Golden Showdown Rule

> **In Texas Hold'em, a Full House ALWAYS beats a Flush.**

No matter how high the Flush is — even an **Ace-high Flush (A♠ K♠ Q♠ J♠ 9♠)** — it **loses** to the lowest possible Full House (such as **2♠ 2♦ 2♣ 3♥ 3♠**, Deuces full of Threes).

### Official Hand Ranking Hierarchy
1. **Royal Flush** (1 in 649,740)
2. **Straight Flush** (1 in 72,193)
3. **Four of a Kind (Quads)** (1 in 4,165)
4. **Full House (Boat)** (1 in 694) — **Higher Rank**
5. **Flush** (1 in 508) — **Lower Rank**
6. **Straight** (1 in 254)
7. **Three of a Kind (Set / Trips)** (1 in 47)
8. **Two Pair** (1 in 21)
9. **One Pair** (1 in 2.37)
10. **High Card** (1 in 1.99)

---

## Why Does Full House Beat Flush? Mathematical Odds

Poker hand rankings are strictly governed by **combinatorial probability**: the rarer the combination, the higher it ranks.

- **Full House Combinations**: 3,744 out of 2,598,960 possible 5-card hands (Probability: **0.1441%**).
- **Flush Combinations**: 5,108 out of 2,598,960 possible 5-card hands (excluding straight flushes) (Probability: **0.1965%**).

Because a Full House is mathematically rarer than a Flush (3,744 vs 5,108 combos), it decisively outranks any Flush.

---

## High-Frequency Table Disputes & Resolution

### Scenario 1: The Ace-High Flush Trap
- **Board**: `K♠ 9♠ 4♠ 4♦ 7♥`
- **Player A**: `A♠ Q♠` (Nut Flush: `A♠ K♠ Q♠ 9♠ 4♠`)
- **Player B**: `K♦ 4♣` (Full House: `4♠ 4♦ 4♣ K♠ K♦`, Fours full of Kings)
- **Ruling**: **Player B wins the entire pot**. Even though Player A holds the nut flush with an Ace kicker, Player B holds a Full House.

### Scenario 2: Paired Board Flush
Whenever the community board pairs, any player holding two pair or trips can make a Full House on the river, instantly beating any player drawing to a flush.

---

## Interactive Evaluator

You can evaluate any 7-card combination (2 hole cards + 5 board cards) with the [FlopKit poker showdown calculator](https://flopkit.com/who-wins/flush-vs-full-house/).

For printable PDF rules and preflop hand charts, visit [FlopKit Printable Poker Cheat Sheet](https://flopkit.com/printable/).

## License
MIT License.
