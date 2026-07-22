---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: sigtuple.com
  spf: true
hosts:
- cert_expires: Mar 27 04:43:08 2027 GMT
  host: www.sigtuple.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sigtuple Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SigTuple, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SigTuple
provider_slug: sigtuple
slug: sigtuple-domain-security
source_filename: sigtuple-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sigtuple.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 27 04:43:08 2027 GMT\n  hsts: false\ndomains:\n- domain: sigtuple.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sigtuple/refs/heads/main/security/sigtuple-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Ai
- Healthcare
- Diagnostics
- Pathology
- Medical Devices
- Microscopy
- Machine Learning
---
