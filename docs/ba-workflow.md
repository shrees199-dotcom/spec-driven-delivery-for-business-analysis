# BA Workflow

This document explains how the Spec-Driven Delivery for Business Analysis project should be used in practice.

## Overview

The workflow is designed to stop requirement drift at the source. It does not assume that discovery notes are enough to build from. Instead, it creates a clean handoff chain:

- raw discovery
- narrative extraction
- contract drafting
- question packet generation
- answer key preparation
- actual build output
- grading and fix routing

## Step 1: Discovery ingestion

Start with real stakeholder material:

- transcript notes
- meeting summaries
- recorded conversations converted to text
- project comments and emails
- open discussion threads

Treat all inputs as raw material until they have been classified.

## Step 2: Narrative extraction

Use the Narrative Extraction Analyst skill to:

- process each session in order
- group statements by the same specific capability
- label items as Confirmed, Exploratory, or Rejected
- maintain speaker attribution
- note cross-session conflicts without resolving them silently

The output is one narrative per distinct capability.

## Step 3: Contract drafting

Only confirmed narratives proceed to the Governor. The Governor creates the Contract using the exact schema and confidence rules required for build execution.

The contract includes:

- trigger
- boundaries
- output schema
- failure plan
- BA provisional calls
- stakeholder question packet

This is the build contract, not a loose feature description.

## Step 4: Gate 1 sign-off

Before engineering builds anything, unresolved items are batched into one Stakeholder Question Packet.

This makes async stakeholder review possible without forcing another live meeting.

## Step 5: Golden Dataset creation

Once the contract is in a workable state, the team writes examples and expected results before any code exists.

This step creates the answer key and includes:

- normal success cases
- negative cases
- flagged ambiguous cases
- known gaps

## Step 6: Gate 2 sign-off

The answer key must be approved as realistic and complete enough to trust before grading.

## Step 7: Real build output required

The process stops at Gate 2.5 until actual build output exists for each example in the answer key.

No grading is allowed based on assumptions.

## Step 8: Grading and fix routing

Once build output is available, the grading step compares the real results against the answer key.

Each failure is classified as one of:

- spec gap
- build gap
- genuinely unclear

If the failure is genuinely unclear, it moves to Gate 3.

## Step 9: Fix management

The workflow supports targeted fixes without resetting the entire project:

- revise only one contract field
- reuse the same answer key for a new build version
- keep prior decisions visible and not silently rewritten

## BA operating principle

The BA's role is to record reality, not invent it. If a decision is not actually stated, it remains open or provisional and is clearly labeled as such.
