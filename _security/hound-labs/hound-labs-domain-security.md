---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hounddiagnostics.com
  spf: true
hosts:
- cert_expires: Oct  6 01:12:06 2026 GMT
  host: hounddiagnostics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hound Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hound Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hound Labs
provider_slug: hound-labs
slug: hound-labs-domain-security
source_filename: hound-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hounddiagnostics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:12:06 2026 GMT\n  hsts: false\ndomains:\n- domain: hounddiagnostics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hound-labs/refs/heads/main/security/hound-labs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Diagnostics
- Drug Testing
- Medical Devices
- Occupational Health
- Workplace Safety
- Cannabis
- Breath Analysis
- Renamed
---
