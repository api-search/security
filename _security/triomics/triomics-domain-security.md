---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: triomics.com
  spf: true
hosts:
- cert_expires: Aug 25 18:08:04 2026 GMT
  host: triomics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Triomics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Triomics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Triomics
provider_slug: triomics
slug: triomics-domain-security
source_filename: triomics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: triomics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 18:08:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: triomics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triomics/refs/heads/main/security/triomics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Oncology
- Healthcare
- Artificial Intelligence
- Clinical Trials
- Electronic Health Records
- Life Sciences
- Cancer
---
