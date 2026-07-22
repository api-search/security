---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mplx.com
  spf: true
hosts:
- cert_expires: Aug 23 00:27:57 2026 GMT
  host: www.mplx.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Markwest Energy Partners Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarkWest Energy Partners, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MarkWest Energy Partners
provider_slug: markwest-energy-partners
slug: markwest-energy-partners-domain-security
source_filename: markwest-energy-partners-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mplx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 00:27:57 2026 GMT\n  hsts: null\ndomains:\n- domain: mplx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/markwest-energy-partners/refs/heads/main/security/markwest-energy-partners-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Energy
- Natural Gas
- Pipeline
- Acquired
- MPLX
---
