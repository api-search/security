---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: prettylitter.com
  spf: true
hosts:
- cert_expires: Nov 11 13:03:48 2026 GMT
  host: prettylitter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pretty Litter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pretty Litter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Pretty Litter
provider_slug: pretty-litter
slug: pretty-litter-domain-security
source_filename: pretty-litter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: prettylitter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 13:03:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: prettylitter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pretty-litter/refs/heads/main/security/pretty-litter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pet Care
- Health Monitoring
- Subscription
- Cat Litter
- Veterinary
---
