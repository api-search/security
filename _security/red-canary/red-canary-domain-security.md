---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: redcanary.com
  spf: true
- caa:
  - 0 issuewild "geotrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: redcanary.co
  spf: true
hosts:
- cert_expires: Oct 14 02:23:33 2026 GMT
  host: redcanary.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 11:11:38 2026 GMT
  host: docs.redcanary.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: go.my.redcanary.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Red Canary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Canary, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Red Canary
provider_slug: red-canary
slug: red-canary-domain-security
source_filename: red-canary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: redcanary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 02:23:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.redcanary.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 11:11:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: go.my.redcanary.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: redcanary.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: redcanary.co\n  dnssec: false\n  caa:\n  - 0 issuewild \"geotrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-canary/refs/heads/main/security/red-canary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cybersecurity
- Managed Detection and Response
- Threat Detection
- Threat Intelligence
- Endpoint Security
- Incident Response
- Security Operations
- Automation
---
