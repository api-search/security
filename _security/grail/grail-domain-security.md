---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: grail.com
  spf: true
hosts:
- cert_expires: Oct 12 04:22:48 2026 GMT
  host: grail.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grail Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grail, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Grail
provider_slug: grail
slug: grail-domain-security
source_filename: grail-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grail.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:22:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: grail.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grail/refs/heads/main/security/grail-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Life Sciences
- Healthcare
- Cancer Detection
- Diagnostics
- Genomics
- Multi-Cancer Early Detection
- Bioinformatics
---
