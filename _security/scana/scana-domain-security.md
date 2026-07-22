---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: scanaenergy.com
  spf: true
hosts:
- cert_expires: Sep 21 21:16:20 2026 GMT
  host: www.scanaenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SCANA Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: SCANA Corporation
provider_slug: scana
slug: scana-domain-security
source_filename: scana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scanaenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 21:16:20 2026 GMT\n  hsts: false\ndomains:\n- domain: scanaenergy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scana/refs/heads/main/security/scana-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Electric Utility
- Energy
- Fortune 1000
- Natural Gas
- South Carolina
- Utility
---
