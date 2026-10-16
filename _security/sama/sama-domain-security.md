---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sama.com
  spf: true
hosts:
- cert_expires: Nov 30 13:00:22 2026 GMT
  host: sama.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sama Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sama, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sama
provider_slug: sama
slug: sama-domain-security
source_filename: sama-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sama.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 13:00:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sama.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sama/refs/heads/main/security/sama-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Data-Annotation
- AI
- B-Corp
- Training-Data
---
