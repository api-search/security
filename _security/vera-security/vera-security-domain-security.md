---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vera.com
  spf: true
hosts:
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: secure.vera.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Vera Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vera Security, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vera Security
provider_slug: vera-security
slug: vera-security-domain-security
source_filename: vera-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: secure.vera.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vera.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vera-security/refs/heads/main/security/vera-security-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Data Security
- Information Rights Management
- Data-Centric Security
- Encryption
- Data Loss Prevention
- Secure Collaboration
- Enterprise Security
---
