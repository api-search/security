---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: reliaquest.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: portal-digitalshadows.com
  spf: true
hosts:
- cert_expires: Nov  3 20:53:47 2026 GMT
  host: reliaquest.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: portal-digitalshadows.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digital Shadows Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digital Shadows, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Digital Shadows
provider_slug: digital-shadows
slug: digital-shadows-domain-security
source_filename: digital-shadows-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reliaquest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 20:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: portal-digitalshadows.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: reliaquest.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: portal-digitalshadows.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digital-shadows/refs/heads/main/security/digital-shadows-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Threat Intelligence
- Digital Risk Protection
- Dark Web Monitoring
- Data Breach
- Brand Protection
- Security Operations
- Vulnerability Intelligence
---
