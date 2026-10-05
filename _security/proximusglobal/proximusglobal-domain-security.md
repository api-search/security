---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: proximusglobal.com
  spf: true
hosts:
- cert_expires: Nov 30 19:22:52 2026 GMT
  host: www.proximusglobal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Proximusglobal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Proximus Global, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Proximus Global
provider_slug: proximusglobal
slug: proximusglobal-domain-security
source_filename: proximusglobal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.proximusglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 19:22:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: proximusglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/proximusglobal/refs/heads/main/security/proximusglobal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Communications
- Digital Identity
- Connectivity
- Fraud Prevention
---
