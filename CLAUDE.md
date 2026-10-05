# AI Instructions

This file provides guidance to AI coding agents (Claude Code, and other
agents reading it via the `AGENTS.md` symlink) when working in this
repository.

## Project overview

This is a personal FreeCAD modeling project, not a software project — there
is no build, lint, or test tooling. The goal is to design a 3D-printable
Steam Deck charger cradle and stand for the EU power adapter, as described
in [README.md](README.md).

It is a remake of a Printables model released under CC BY-NC-SA, so this
repository must stay under the same license and keep crediting the original
(see the README).

## Repository structure

- `cad/` — FreeCAD source file (`.FCStd`).
- `exports/` — 3MF export for slicing and printing.
- `images/` — reference photo, renders, slicer screenshot and print photos
  (PNG).

## Language

Write everything in this repository — README, commit messages, code
comments, docs — in English only. Conversation with the user can be in
whichever language they use.

## Working with the FreeCAD file

- `.FCBak` backup files and the `backup/` directory are gitignored — never
  commit them.
- The `.FCStd` file is a binary FreeCAD document; it can't be reviewed as a
  text diff, so describe what changed in the commit message instead.
