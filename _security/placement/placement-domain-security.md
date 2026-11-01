---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: placement.com
  spf: true
hosts:
- cert_expires: Dec 22 05:44:34 2026 GMT
  host: www.placement.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Placement Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Placement, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Placement
provider_slug: placement
slug: placement-domain-security
source_filename: placement-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.placement.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 05:44:34 2026 GMT\n  hsts: false\ndomains:\n- domain: placement.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/placement/security/placement-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- AI Training
- Conversation Intelligence
- Sales Enablement
- Employee Training
- Leadership Development
- Call Scoring
---
