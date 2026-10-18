---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: latii.com
  spf: true
hosts:
- cert_expires: Jan  9 11:34:32 2027 GMT
  host: latii.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Latii Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Latii, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Latii
provider_slug: latii
slug: latii-domain-security
source_filename: latii-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: latii.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 11:34:32 2027 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: latii.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/latii/refs/heads/main/security/latii-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Software-as-a-Service
- Window-Doors
- Marketplace
- Artificial Intelligence
---
