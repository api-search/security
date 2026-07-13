---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: presidio.com
  spf: true
hosts:
- cert_expires: Sep 25 10:04:28 2026 GMT
  host: www.presidio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.presidio.com
  https: false
- host: api.presidio.com
  https: false
kind: domain-security
layout: security
method: probed
name: Presidio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Presidio Inc, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Presidio Inc
provider_slug: presidio
slug: presidio-domain-security
source_filename: presidio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.presidio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 10:04:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.presidio.com\n  https: false\n- host: api.presidio.com\n  https: false\ndomains:\n- domain: presidio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/presidio/refs/heads/main/security/presidio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- IT Solutions
- Cloud
- Security
---
