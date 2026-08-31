---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: windward.ai
  spf: true
hosts:
- cert_expires: Oct  8 13:32:42 2026 GMT
  host: windward.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Windward Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Windward, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Windward
provider_slug: windward-ai
slug: windward-ai-domain-security
source_filename: windward-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: windward.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 13:32:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: windward.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windward-ai/refs/heads/main/security/windward-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Maritime
- Maritime AI
- Maritime Domain Awareness
- Vessel Intelligence
- Vessel Risk
- Sanctions Screening
- Trade Compliance
- Trade Intelligence
- Risk and Compliance
- Deceptive Shipping
- Ship-to-Ship Transfer
- Container Tracking
- Supply Chain Visibility
- Behavioral Analytics
- Remote Sensing
- AIS
- GeoINT
- IUU Fishing
- Defense and Intelligence
- Border Security
- GraphQL
---
