---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: autobahntx.com
  spf: true
hosts:
- cert_expires: Aug 23 13:26:20 2026 GMT
  host: www.autobahntx.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autobahn Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autobahn Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Autobahn Therapeutics
provider_slug: autobahn-therapeutics
slug: autobahn-therapeutics-domain-security
source_filename: autobahn-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.autobahntx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 13:26:20 2026 GMT\n  hsts: false\ndomains:\n- domain: autobahntx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autobahn-therapeutics/refs/heads/main/security/autobahn-therapeutics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biopharmaceutical
- Biotechnology
- Central Nervous System
- Neuroscience
- Drug Development
- Regenerative Medicine
- Small Molecule
- Clinical Stage
- Healthcare
---
