---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zenput.com
  spf: true
hosts:
- cert_expires: Sep 20 11:12:36 2026 GMT
  host: www.zenput.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:28:56 2026 GMT
  host: developer.zenput.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenput Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenput, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Zenput
provider_slug: zenput
slug: zenput-domain-security
source_filename: zenput-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zenput.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:12:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.zenput.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:28:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zenput.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenput/refs/heads/main/security/zenput-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Restaurant Operations
- Operations Execution
- Food Safety
- Compliance
- Task Management
- Convenience Stores
- Field Operations
- Restaurant Technology
---
