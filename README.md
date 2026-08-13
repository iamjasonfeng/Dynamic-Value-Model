# Dynamic-Value-Model

Dynamic Value Model for ARC-AGI-3

[PDF](https://iamjasonfeng.github.io/Dynamic-Value-Model/dynamic_value_model_for_arc_agi_3.pdf)

Abstract

This paper presents Dynamic Value Model (DVM), a lightweight test-time method for interactive agents.
During every action call, the acting model maintains a visible, persistent JSON value model that assigns and
continually revises value judgments for candidate hypotheses, policies, subgoals, tests, actions, and possible
states. It estimates value across immediate, short-term, medium-term, long-term, and ultra-long-term
horizons while considering information value, potential upside and downside, risk, recoverability, evidence,
uncertainty, and whether that value transfers to later levels. Before acting, the model explains how its
current value judgments inform the next action. DVM complements rather than replaces the world model:
the world model represents what the environment contains and how it behaves, while the value model
represents what is worth pursuing and why. It requires no weight updates, auxiliary model calls, search
branches, or environment copies. On the 25 public ARC-AGI-3 games, DeepSeek V4 Flash with DVM

scored 14.38%, compared with 11.02% for Policy Superposition and 6.01% for the baseline. These single-
run comparisons are preliminary; the earlier two runs also shared a temporary API-balance outage that did

not affect DVM.
