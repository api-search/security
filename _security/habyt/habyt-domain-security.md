---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: habyt.com
  spf: true
hosts:
- cert_expires: Aug 22 10:43:31 2026 GMT
  host: www.habyt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Habyt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Habyt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Habyt
provider_slug: habyt
slug: habyt-domain-security
source_filename: habyt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.habyt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 10:43:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: habyt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/habyt/refs/heads/main/security/habyt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Real Estate
- Housing
- Co-Living
- Flexible Living
- Hospitality
- Property
---
