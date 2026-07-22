---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: govwell.com
  spf: true
hosts:
- cert_expires: Oct 15 06:33:42 2026 GMT
  host: govwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Govwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GovWell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GovWell
provider_slug: govwell
slug: govwell-domain-security
source_filename: govwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: govwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 06:33:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: govwell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/govwell/refs/heads/main/security/govwell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government
- GovTech
- Local Government
- Permitting
- Licensing
- Code Enforcement
- Planning and Zoning
---
