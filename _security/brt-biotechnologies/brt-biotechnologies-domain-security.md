---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: brtbio.com
  spf: true
hosts:
- cert_expires: Nov 11 09:03:15 2026 GMT
  host: brtbio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brt Biotechnologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BRT Biotechnologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BRT Biotechnologies
provider_slug: brt-biotechnologies
slug: brt-biotechnologies-domain-security
source_filename: brt-biotechnologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: brtbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 09:03:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: brtbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brt-biotechnologies/refs/heads/main/security/brt-biotechnologies-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Biotechnology
- Drug Discovery
- Macrocycles
- Therapeutics
- Company
---
