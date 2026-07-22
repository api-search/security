---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gebeya.com
  spf: true
hosts:
- cert_expires: Oct 13 00:08:01 2026 GMT
  host: www.gebeya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gebeya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gebeya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gebeya
provider_slug: gebeya
slug: gebeya-domain-security
source_filename: gebeya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gebeya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 00:08:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gebeya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gebeya/refs/heads/main/security/gebeya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketplace
- Talent
- Africa
- SaaS
- Marketplace as a Service
- Artificial Intelligence
- Ethiopia
---
