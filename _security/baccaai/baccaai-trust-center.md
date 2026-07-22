---
certifications:
- SOC 2 Type I
- SOC 2 Type II
- GDPR
description: ''
kind: trust-center
layout: security
name: Baccaai Trust Center
name_suffix: Trust Center
overview: Bacca.ai maintains a public trust center documenting SOC 2 Type I, SOC 2 Type II, and GDPR compliance.
provider_name: Bacca.ai
provider_slug: baccaai
slug: baccaai-trust-center
source_filename: baccaai-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nprobe: false\nsource: https://www.bacca.ai/legals/security-and-privacy-whitepaper\nurl: https://trust.bacca.ai/\ncertifications:\n- SOC 2 Type I\n- SOC 2 Type II\n- GDPR\nframeworks:\n- name: SOC 2 Type I & Type II\n  status: attested\n  evidence: Bacca maintains a SOC 2 Type I & Type II attestation; report available via the Trust Center.\n- name: GDPR\n  status: compliant\n  evidence: GDPR referenced for data-retention policy; continuously evaluates emerging regulatory frameworks.\ncontrols:\n  tenancy: single-tenant; strict logical and physical separation of data per customer, no cross-customer data pollination\n  hosting: Google Cloud Platform (GCP)\n  encryption_at_rest: all customer datastores encrypted at rest; row-level encryption for sensitive data\n  encryption_in_transit: TLS 1.2 or higher; HSTS enabled\n  key_management: GCP KMS with keys stored in Hardware Security Modules (HSMs)\n  access: least-privilege, role-based access,\
  \ automatic deprovisioning on termination, phishing-resistant MFA\n  testing: SAST, SCA, DAST vulnerability scanning; continuous external attack surface management\n  data_retention: 30-day retention window for raw incident data; anonymization for knowledge aggregation\nevidence:\n- source: https://www.bacca.ai/legals/security-and-privacy-whitepaper\n  keywords: [soc 2 type i, soc 2 type ii, gdpr, encryption at rest, gcp kms]\n- source: https://trust.bacca.ai/\n  kind: trust-center\nnotes: Trust Center portal is JavaScript-rendered (trust.bacca.ai); certifications confirmed from the public Security & Privacy Whitepaper.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baccaai/refs/heads/main/security/baccaai-trust-center.yml
summary_line: SOC 2 Type I, SOC 2 Type II, GDPR
tags:
- Company
- Ai
- Site Reliability Engineering
- Incident Management
- Observability
- DevOps
- AI Agent
- Root Cause Analysis
- Cloud
trust_url: https://trust.bacca.ai/
---
