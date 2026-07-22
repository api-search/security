---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: behance.net
  spf: true
hosts:
- cert_expires: Oct  5 01:08:23 2026 GMT
  host: behance.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Behance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Behance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Behance
provider_slug: behance
slug: behance-domain-security
source_filename: behance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: behance.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 01:08:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: behance.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/behance/refs/heads/main/security/behance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Portfolio
- Creative Network
- Design Community
- Adobe
- Creative Cloud
- Content
---
