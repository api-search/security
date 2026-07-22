---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: osisoft.com
  spf: true
hosts:
- cert_expires: Oct 18 18:07:13 2026 GMT
  host: www.osisoft.com
  hsts: true
  hsts_max_age: 15638400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Osisoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OSIsoft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: OSIsoft
provider_slug: osisoft
slug: osisoft-domain-security
source_filename: osisoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.osisoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 18:07:13 2026 GMT\n  hsts: true\n  hsts_max_age: 15638400\ndomains:\n- domain: osisoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/osisoft/refs/heads/main/security/osisoft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Industrial
- Operational Data
- Time Series
- IIoT
- PI System
- Manufacturing
---
