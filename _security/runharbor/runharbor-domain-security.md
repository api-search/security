---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: runharbor.com
  spf: true
hosts:
- cert_expires: Oct 16 11:24:09 2026 GMT
  host: runharbor.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runharbor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Runharbor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Runharbor
provider_slug: runharbor
slug: runharbor-domain-security
source_filename: runharbor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runharbor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:24:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: runharbor.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runharbor/refs/heads/main/security/runharbor-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Clinical Trials
- Healthcare
- Contract Research Organization
- Electronic Data Capture
- Life Sciences
- Compliance
- Artificial Intelligence
- eClinical
---
