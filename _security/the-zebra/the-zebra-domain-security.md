---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: thezebra.com
  spf: true
hosts:
- cert_expires: Oct 12 03:46:37 2026 GMT
  host: www.thezebra.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: The Zebra Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Zebra, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: The Zebra
provider_slug: the-zebra
slug: the-zebra-domain-security
source_filename: the-zebra-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.thezebra.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 12 03:46:37 2026 GMT\n  hsts: null\ndomains:\n- domain: thezebra.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-zebra/refs/heads/main/security/the-zebra-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Consumer
- Insurance
- Insurance Comparison
- Marketplace
- Auto Insurance
---
