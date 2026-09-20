# Cognitive Adaptive State Specification

## Overview

Chameleon uses an adaptive cognitive-friendly state to reduce unnecessary visual competition while keeping essential dashboard information available.

The design uses two primary interface states:

- **Normal State** — standard dashboard presentation.
- **Cognitive-Friendly State** — adapted presentation intended to make important information easier to scan and reduce unnecessary visual competition.

## State Changes

| Area | Normal State | Cognitive-Friendly State |
|---|---|---|
| KPI cards | Value, change, and sparkline | Value and change are emphasized; redundant sparkline removed |
| Sales Performance | Standard bar spacing | Increased separation between monthly bars |
| Recent Activity | Standard text hierarchy | Clearer primary/secondary text hierarchy and more breathing room |
| Recent Transactions | Standard table hierarchy | Clearer column hierarchy, stronger amounts/status, quieter supporting dates |
| Navigation | Familiar sidebar/header | Preserved to maintain familiarity |
| Focus indicator | Standard dashboard | Focus Mode indicator identifies the adaptive state |

## Design Principle

The cognitive-friendly state does not simply remove information. It reduces redundancy and visual competition while preserving information needed to understand and use the dashboard.

## Prototype Trigger

The transition is demonstrated through a simulated **High Cognitive Load Detected** condition in Figma.