---
certifications:
- SOC 2
- HIPAA
description: ''
kind: trust-center
layout: security
name: Shadowfax Trust Center
name_suffix: Trust Center
overview: Shadowfax AI maintains a public trust center documenting SOC 2 and HIPAA compliance.
provider_name: Shadowfax AI
provider_slug: shadowfax
slug: shadowfax-trust-center
source_filename: shadowfax-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://trust.shadowfax.ai/\nurl: https://trust.shadowfax.ai/\nname: Shadowfax AI Trust Center\nnote: >-\n  Self-hosted trust center at trust.shadowfax.ai (HTTP 200, 429KB, browser\n  User-Agent required — a default crawler UA is answered with a CloudFront 403).\n  The page states the company was founded in 2025 and publishes a security\n  contact, a compliance list, a control inventory, a policy library and a\n  named subprocessor list. Corrected by hand after the automated probe:\n  probe-security-programs.py captured HIPAA as an achieved certification, but\n  the page marks it \"Coming soon\" — only SOC 2 is claimed as attained.\ncertifications:\n- name: SOC 2\n  status: compliant\n  evidence: 'Compliances table: \"SOC 2 — Compliant\"'\n- name: HIPAA\n  status: coming-soon\n  evidence: 'Compliances table: \"HIPAA — Coming soon\"'\n  note: Announced, not attained. Do not count this as a held certification.\ncontrol_families:\n\
  - product-security\n- data-security\n- network-security\n- app-security\n- endpoint-security\n- corporate-security\npolicies:\n  published: false\n  note: >-\n    A policy library is listed (System Description, Personal Data Breach\n    Notification Procedure, PHI Data Breach Notification Procedure, Physical &\n    Environmental Security, SDLC Procedure, and \"+39 more\") but the documents\n    themselves are behind a \"Request access\" gate.\nsubprocessors:\n- name: PostHog\n  category: Analytics\n  region: United States of America\n- name: Cloudflare\n  category: Hosting Providers\n  region: United States of America\n- name: Anthropic\n  category: Artificial Intelligence\n  region: United States of America\n- name: GCP\n  category: IT infrastructure\n  region: United States of America\n- name: Sentry\n  category: Analytics\n  region: United States of America\n- name: OpenAI\n  category: Artificial Intelligence\n  region: United States of America\nevidence:\n- url: https://trust.shadowfax.ai/\n\
  \  status: 200\n  note: 200 with a browser User-Agent; 403 (CloudFront) with a default crawler UA.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shadowfax/refs/heads/main/security/shadowfax-trust-center.yml
summary_line: SOC 2, HIPAA
tags:
- Company
- Analytics
- Business Intelligence
- Artificial Intelligence
- Data
- Agentic Analytics
- Data Engineering
- SaaS
trust_url: https://trust.shadowfax.ai/
---
