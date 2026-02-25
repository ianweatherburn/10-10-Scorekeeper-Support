<p align="center">
  <img src="Resources/Images/cards_logo_transparent.png" alt="Judgement Scorekeeper Logo" width="220" />
</p>

# 10-10 Scorekeeper
### Copyright 2026 by Ian Weatherburn
ianweatherburn@gmail.com

## Description

10-10 (also known as "Judgement", "Oh Pshaw!" or "O Hell") is a popular trick-taking card game for 3-7 players that combines strategy, skill, and a bit of luck.
Players must accurately predict how many tricks they'll win each round, making it both challenging and exciting for card game enthusiasts.

**Objective**: Score the most points by accurately bidding the number of tricks you'll win in each round. Exact bids earn bonus points, while missed bids may result in penalties.

## Overview

A SwiftUI scorekeeper app for the trick-taking card game **Judgement**.
Scorekeeper tracks bids, tricks made, scores, dealer rotation, and trump suits across all rounds of a Judgement game. It supports 3–7 players, four different scoring modes, and persists game state so a game can be resumed if the app is closed. The Scorekeeper app also tracks player statistics across games.
This app does **not** implement the card game itself; it is a companion scorekeeper for players at a physical table.

## Key Features

- **Player Management:** Add, select, and order players via drag-and-drop to reflect table seating
- **Automatic Round Calculation:** Adjusts rounds and max cards based on player count and a 52-card deck constraint
- **Trump Rotation:** Hearts -> Clubs -> Diamonds -> Spades -> No Trumps, cycling across all rounds
- **Dealer Rotation:** Tracks and animates the current dealer each round; bidding starts after the dealer
- **Bid Validation:** Enforces the "last bidder cannot make total equal round number" rule
- **Made Tricks Validation:** Ensures total made tricks equals the card count for the round
- **Four Scoring Modes:** "Standard", "Penalty", "Progressive" and "Exact"
- **Running Score Display:** Total scores visible at all times with a scrollable round history which is also editable to correct any past mistakes
- **Game Persistence:** Active game and player data persisted with Point-Free Sharing (`@Shared` file/app storage)
- **Winner Announcement:** Ranked results with success haptics
- **Settings:** Scoring mode, player count limits, dark/light mode override, reset all data
- **About Screen:** App info, logo, and comprehensive rules for all scoring modes
- **Live Widget:** Home Screen live widget showing current round, trump card, scoring mode, number of cards to be dealt, player scores, and current dealer
- **Dynamic Island:** Large and Small dynamic islands showing current round, trumps, cards to be dealt and score details
- **Watch OS Live Stack:** Live Stack on Apple Watch showing current round, trumps and number of cards to be dealt

## Supports

- iOS 26.0+
- iPhone portrait orientation only
- iPhone / Apple Watch Widgets and Stacks
