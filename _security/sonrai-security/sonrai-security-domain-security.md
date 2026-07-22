---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sonraisecurity.com
  spf: true
hosts:
- cert_expires: Aug 24 03:42:57 2026 GMT
  host: sonraisecurity.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sonrai Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonrai Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sonrai Security
provider_slug: sonrai-security
slug: sonrai-security-domain-security
source_filename: sonrai-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sonraisecurity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 03:42:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: sonraisecurity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sonrai-security/refs/heads/main/security/sonrai-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cloud Security
- Identity and Access Management
- CIEM
- Cloud Permissions
- Least Privilege
- GraphQL
- IAM
---
