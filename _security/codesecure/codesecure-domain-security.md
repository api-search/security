---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: codesecure.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: adacore.com
  spf: true
hosts:
- cert_expires: Oct  1 17:15:24 2026 GMT
  host: codesecure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 05:49:57 2026 GMT
  host: www.adacore.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codesecure Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeSecure, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: CodeSecure
provider_slug: codesecure
slug: codesecure-domain-security
source_filename: codesecure-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codesecure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 17:15:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.adacore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 05:49:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: codesecure.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: adacore.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codesecure/refs/heads/main/security/codesecure-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Application Security
- Static Analysis
- SAST
- Software Composition Analysis
- SBOM
- DevSecOps
- Code Quality
- Security
---
