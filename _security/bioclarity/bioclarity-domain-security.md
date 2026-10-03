---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bioclarity.com
  spf: true
hosts:
- cert_expires: Dec 24 10:56:32 2026 GMT
  host: www.bioclarity.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bioclarity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for bioClarity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: bioClarity
provider_slug: bioclarity
slug: bioclarity-domain-security
source_filename: bioclarity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bioclarity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 10:56:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: bioclarity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bioclarity/refs/heads/main/security/bioclarity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Skincare
- Vegan
- Plant-Based
- Beauty
- E-Commerce
---
