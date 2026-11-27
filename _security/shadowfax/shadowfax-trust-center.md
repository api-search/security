---
certification_count: 1
certifications:
- SOC 2
description: ''
kind: trust-center
layout: security
name: Shadowfax AI Trust Center
name_suffix: Trust Center
overview: Shadowfax AI maintains a public trust center documenting SOC 2 compliance.
provider_name: Shadowfax AI
provider_slug: shadowfax
slug: shadowfax-trust-center
source_filename: shadowfax-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://trust.shadowfax.ai/\nurl: https://trust.shadowfax.ai/\nname: Shadowfax AI Trust Center\nnote: 'Self-hosted trust center at trust.shadowfax.ai (HTTP 200, 429KB, browser User-Agent required —\n  a default crawler UA is answered with a CloudFront 403). The page states the company was founded in\n  2025 and publishes a security contact, a compliance list, a control inventory, a policy library and\n  a named subprocessor list. Corrected by hand after the automated probe: probe-security-programs.py captured\n  HIPAA as an achieved certification, but the page marks it \"Coming soon\" — only SOC 2 is claimed as attained.'\ncertifications:\n- name: SOC 2\n  status: compliant\n  evidence: 'Compliances table: \"SOC 2 — Compliant\"'\ncontrol_families:\n- product-security\n- data-security\n- network-security\n- app-security\n- endpoint-security\n- corporate-security\npolicies:\n  published: false\n  note: A policy library is listed\
  \ (System Description, Personal Data Breach Notification Procedure, PHI\n    Data Breach Notification Procedure, Physical & Environmental Security, SDLC Procedure, and \"+39 more\")\n    but the documents themselves are behind a \"Request access\" gate.\nsubprocessors:\n- name: PostHog\n  category: Analytics\n  region: United States of America\n- name: Cloudflare\n  category: Hosting Providers\n  region: United States of America\n- name: Anthropic\n  category: Artificial Intelligence\n  region: United States of America\n- name: GCP\n  category: IT infrastructure\n  region: United States of America\n- name: Sentry\n  category: Analytics\n  region: United States of America\n- name: OpenAI\n  category: Artificial Intelligence\n  region: United States of America\nevidence:\n- url: https://trust.shadowfax.ai/\n  status: 200\n  note: 200 with a browser User-Agent; 403 (CloudFront) with a default crawler UA.\ncertifications_in_progress:\n- HIPAA\ncertification_quotes:\n  HIPAA: Compliant | HIPAA\
  \ | Coming soon | Controls | Details | Product security | Situational A\ncertifications_checked:\n  date: '2026-11-11'\n  by: probe-security-programs.classify_certs\n  note: a certification is listed only when the trust page states it as held (roadmap#1133)\n"
source_yaml_url: https://artifacts.apis.io/shadowfax/security/shadowfax-trust-center.yml
summary_line: SOC 2
tags:
- Company
- Analytics
- Business Intelligence
- Artificial Intelligence
- Data
- Agentic Analytics
- Data Engineering
- Software-as-a-Service
trust_url: https://trust.shadowfax.ai/
---
