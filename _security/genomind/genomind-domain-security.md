---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: genomind.com
  spf: true
hosts:
- cert_expires: Oct  1 02:52:43 2026 GMT
  host: genomind.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genomind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genomind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Genomind
provider_slug: genomind
slug: genomind-domain-security
source_filename: genomind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: genomind.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:52:43 2026 GMT\n  hsts: false\ndomains:\n- domain: genomind.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genomind/refs/heads/main/security/genomind-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Health
- Healthcare
- Genomics
- Pharmacogenomics
- Precision Medicine
- Mental Health
- Diagnostics
- Laboratory
- Clinical Decision Support
- HIPAA
- EHR Integration
---
