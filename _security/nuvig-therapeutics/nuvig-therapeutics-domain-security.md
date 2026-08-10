---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nuvigtx.com
  spf: true
hosts:
- cert_expires: Oct 11 21:23:43 2026 GMT
  host: nuvigtx.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuvig Therapeutics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nuvig Therapeutics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nuvig Therapeutics
provider_slug: nuvig-therapeutics
slug: nuvig-therapeutics-domain-security
source_filename: nuvig-therapeutics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nuvigtx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 21:23:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: nuvigtx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuvig-therapeutics/refs/heads/main/security/nuvig-therapeutics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Immunology
- Autoimmune Disease
- Therapeutics
- Clinical Trials
- Life Sciences
- United States
---
