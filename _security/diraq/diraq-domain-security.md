---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: diraq.com
  spf: true
hosts:
- cert_expires: Oct 16 02:23:29 2026 GMT
  host: www.diraq.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diraq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diraq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Diraq
provider_slug: diraq
slug: diraq-domain-security
source_filename: diraq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.diraq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 02:23:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: diraq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diraq/refs/heads/main/security/diraq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Quantum Computing
- Semiconductors
- Deep Tech
- Hardware
- Research
- Australia
---
