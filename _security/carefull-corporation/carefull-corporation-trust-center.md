---
certifications:
- SOC 2
description: ''
kind: trust-center
layout: security
name: Carefull Corporation Trust Center
name_suffix: Trust Center
overview: Carefull Corporation maintains a public trust center documenting SOC 2 compliance.
provider_name: Carefull Corporation
provider_slug: carefull-corporation
slug: carefull-corporation-trust-center
source_filename: carefull-corporation-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://getcarefull.com/security-practices\nurl: https://getcarefull.com/security-practices\ncertifications:\n- SOC 2\nevidence:\n- source: https://getcarefull.com/security-practices\n  detail: 'Carefull states it is the first financial caregiving service to receive\n    its SOC 2 certification; independently audited with an unqualified (clean) opinion,\n    zero exceptions. SOC 2 report available on request via care@getcarefull.com.'\nsecurity_posture:\n  encryption_at_rest: AES-256 (per-object keys) for the Carefull Vault\n  encryption_in_transit: TLS with HSTS\n  tokenization: proprietary aliasing system removes sensitive data from core systems\n  data_separation: personal and financial transaction data held in separate databases\n  hosting: AWS across at least three separate geographic locations\n  credentials: banking credentials never stored; view-only aggregation via Plaid, MX, and Finicity\n  ssn_protection: partners\
  \ with Iris and Equifax; SSN never stored with account data\ncontact: care@getcarefull.com\nnotes: No public bug bounty, responsible-disclosure policy, /.well-known/security.txt, or security@ address was found (all /.well-known/* paths return the SPA HTML shell, i.e. soft-404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carefull-corporation/refs/heads/main/security/carefull-corporation-trust-center.yml
summary_line: SOC 2
tags:
- Company
- Fintech
- Financial Safety
- Fraud Detection
- Identity Theft Protection
- Elder Care
- Financial Caregiving
- Account Monitoring
- Consumer Finance
trust_url: https://getcarefull.com/security-practices
---
