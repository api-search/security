---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: clearlabs.com
  spf: true
hosts:
- cert_expires: Oct  2 19:33:45 2026 GMT
  host: clearlabs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clearlabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clear Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Clear Labs
provider_slug: clearlabs
slug: clearlabs-domain-security
source_filename: clearlabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clearlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:33:45 2026 GMT\n  hsts: false\ndomains:\n- domain: clearlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clearlabs/refs/heads/main/security/clearlabs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Genomics
- Sequencing
- Infectious Disease
- Food Safety
- Oncology
- Diagnostics
- Biotechnology
---
