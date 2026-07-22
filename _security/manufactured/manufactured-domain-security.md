---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: manufactured.com
  spf: true
hosts:
- host: manufactured.com
  https: false
kind: domain-security
layout: security
method: probed
name: Manufactured Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Manufactured, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Manufactured
provider_slug: manufactured
slug: manufactured-domain-security
source_filename: manufactured-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: manufactured.com\n  https: false\ndomains:\n- domain: manufactured.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/manufactured/refs/heads/main/security/manufactured-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Company
- Manufacturing
- Supply Chain
- Sourcing
- Procurement
- Hardware
- Production Financing
- Vendor Management
- AI Assistant
---
