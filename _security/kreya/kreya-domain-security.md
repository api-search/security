---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kreya.app
  spf: true
hosts:
- cert_expires: Oct  4 15:13:02 2026 GMT
  host: kreya.app
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kreya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kreya, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kreya
provider_slug: kreya
slug: kreya-domain-security
source_filename: kreya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kreya.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 15:13:02 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: kreya.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kreya/refs/heads/main/security/kreya-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Client
- Developer Tools
- gRPC
- REST
---
