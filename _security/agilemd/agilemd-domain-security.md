---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agilemd.com
  spf: true
hosts:
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: www.agilemd.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agilemd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agilemd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Agilemd
provider_slug: agilemd
slug: agilemd-domain-security
source_filename: agilemd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agilemd.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\ndomains:\n- domain: agilemd.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agilemd/refs/heads/main/security/agilemd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- Clinical Decision Support
- Predictive Analytics
- EHR Integration
- Clinical Pathways
- Patient Safety
- Machine Learning
- Medical Device
---
