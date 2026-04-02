# Protein-Ligand Docking

`protein-ligand-docking` is a research-oriented OpenClaw skill for evaluating whether a ligand may plausibly bind a protein target and whether docking is worth pursuing further.

It is designed for questions such as:

- Can ligand X plausibly bind protein Y?
- Is an inhibitor likely to be selective between bacterial and human homologs?
- Is sequence or structural divergence already large enough to stop before docking?

## What This Skill Covers

- target sequence retrieval
- PDB structure search
- homolog conservation screening
- AlphaFold-Multimer support through Colab
- model-quality review with pLDDT and PAE
- AutoDock Vina docking
- structured interpretation and reporting

## Repository Structure

- `SKILL.md`: core skill instructions for the AI runtime
- `agents/openai.yaml`: optional Codex/OpenAI-style interface metadata
- `references/`: thresholds, QC rules, and helper materials
- `scripts/`: local workflow scripts for alignment, model assessment, docking, and reporting

## Notes

- This skill is intended for computational hypothesis generation, not proof of molecular binding.
- Docking results should be interpreted together with model confidence and biological plausibility.
- Experimental validation remains essential.

## Current Release Focus

The latest local revision simplifies the skill structure, separates detailed thresholds into reference material, and makes the decision points clearer for real-world biomedical use.
