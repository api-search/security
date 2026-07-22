---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gozauber.com
  spf: true
hosts:
- cert_expires: Oct 11 20:26:02 2026 GMT
  host: gozauber.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zauber Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zauber, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Zauber
provider_slug: zauber
slug: zauber-domain-security
source_filename: zauber-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gozauber.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 20:26:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gozauber.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zauber/refs/heads/main/security/zauber-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Freight Forwarding
- Logistics
- AI Agents
- Supply Chain
- Automation
- Sea Freight
- Air Freight
---
