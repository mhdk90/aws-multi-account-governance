# AWS Landing Zone & Multi-Account Governance

## Overview
This project demonstrates a governance-focused AWS foundation using AWS Organizations and Service Control Policies (SCPs), with CloudFormation used as Infrastructure as Code.

## Goal
Build a secure multi-account baseline that can be used as a starting point for a landing zone with centralized governance, access control, and audit readiness.

## Current Scope
- Baseline SCP in CloudFormation
- Multi-account governance starter structure
- Documentation for future CloudTrail and audit controls

## Repository Structure
- `cloudformation/` – CloudFormation templates
- `docs/` – architecture notes and design decisions

## Current Template
- `baseline-scp.yml` – creates an Organizations SCP that can be attached to a Root, OU, or Account

## Deployment Notes
- Deploy from the AWS Organizations management account or a delegated administrator
- The policy type must already be enabled in the organization
- Replace the target ID parameter with the correct Root, OU, or account ID

## Security Notes
- No secrets are stored in this repository
- Environment-specific values should be passed as parameters
- This project is intended as a governance baseline, not a complete landing zone

## Roadmap
- Add CloudTrail baseline
- Add architecture diagram
- Add design decisions
- Add CI lint workflow

## What I Learned
- How AWS Organizations policies can be defined in CloudFormation
- How to structure governance projects for GitHub
- How to document cloud architecture in a recruiter-friendly way
