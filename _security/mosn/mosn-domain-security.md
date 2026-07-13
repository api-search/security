---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mosn.io
  spf: false
hosts:
- cert_expires: Jan  5 23:59:59 2027 GMT
  host: mosn.io
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mosn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOSN, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: MOSN
provider_slug: mosn
slug: mosn-domain-security
source_filename: mosn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mosn.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: mosn.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mosn/refs/heads/main/security/mosn-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Service Mesh
- Proxy
- API Gateway
- Cloud Native
- Open Source
---
