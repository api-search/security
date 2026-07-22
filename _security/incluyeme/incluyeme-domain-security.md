---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: incluyeme.com
  spf: true
hosts:
- cert_expires: Sep  3 01:57:17 2026 GMT
  host: incluyeme.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Incluyeme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Incluyeme, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Incluyeme
provider_slug: incluyeme
slug: incluyeme-domain-security
source_filename: incluyeme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: incluyeme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 01:57:17 2026 GMT\n  hsts: false\ndomains:\n- domain: incluyeme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incluyeme/refs/heads/main/security/incluyeme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Disability Inclusion
- Employment
- Recruiting
- Job Board
- HR Tech
- Accessibility
- Diversity Equity and Inclusion
- Social Enterprise
- Latin America
- Training
---
