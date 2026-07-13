---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: automox.com
  spf: true
hosts:
- cert_expires: Sep 17 13:03:46 2026 GMT
  host: www.automox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 23:59:59 2026 GMT
  host: developer.automox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 08:16:34 2026 GMT
  host: console.automox.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Automox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automox, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Automox
provider_slug: automox
slug: automox-domain-security
source_filename: automox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.automox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 13:03:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.automox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: console.automox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 08:16:34 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: automox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automox/refs/heads/main/security/automox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Endpoint Management
- Patch Management
- IT Operations
- Device Management
- Configuration Management
- Security
---
