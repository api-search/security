---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: advanced-ionics.com
  spf: true
hosts:
- cert_expires: Oct 28 15:24:19 2026 GMT
  host: advanced-ionics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Advanced Ionics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advanced Ionics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Advanced Ionics
provider_slug: advanced-ionics
slug: advanced-ionics-domain-security
source_filename: advanced-ionics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: advanced-ionics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 15:24:19 2026 GMT\n  hsts: false\ndomains:\n- domain: advanced-ionics.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advanced-ionics/refs/heads/main/security/advanced-ionics-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Energy
- Hydrogen
- Clean Energy
- Electrolyzer
- Manufacturing
- Industrial
- Hardware
- Climate Tech
---
