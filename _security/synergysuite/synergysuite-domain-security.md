---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: synergysuite.com
  spf: true
hosts:
- cert_expires: Oct  3 07:43:06 2026 GMT
  host: www.synergysuite.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Synergysuite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SynergySuite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SynergySuite
provider_slug: synergysuite
slug: synergysuite-domain-security
source_filename: synergysuite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.synergysuite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:43:06 2026 GMT\n  hsts: null\ndomains:\n- domain: synergysuite.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synergysuite/refs/heads/main/security/synergysuite-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Restaurants
- Hospitality
- Restaurant Management
- Back Of House
- Inventory Management
- Food Safety
- Workforce Scheduling
- Point Of Sale Integration
- Business Intelligence
- EDI
- SaaS
---
