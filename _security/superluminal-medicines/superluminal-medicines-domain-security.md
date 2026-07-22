---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: superluminalrx.com
  spf: true
hosts:
- cert_expires: Aug 27 17:18:47 2026 GMT
  host: www.superluminalrx.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superluminal Medicines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superluminal Medicines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Superluminal Medicines
provider_slug: superluminal-medicines
slug: superluminal-medicines-domain-security
source_filename: superluminal-medicines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.superluminalrx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:18:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: superluminalrx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superluminal-medicines/refs/heads/main/security/superluminal-medicines-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotech Therapeutics
- Drug Discovery
- Artificial Intelligence
- Small Molecule Therapeutics
- GPCR
- Life Sciences
---
