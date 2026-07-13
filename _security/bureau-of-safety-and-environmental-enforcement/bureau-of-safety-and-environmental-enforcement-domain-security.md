---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: bsee.gov
  spf: true
hosts:
- cert_expires: Aug 28 21:44:11 2026 GMT
  host: www.bsee.gov
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 16 23:59:59 2027 GMT
  host: www.data.bsee.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: timsweb.bsee.gov
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bureau Of Safety And Environmental Enforcement Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bureau of Safety and Environmental Enforcement, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bureau of Safety and Environmental Enforcement
provider_slug: bureau-of-safety-and-environmental-enforcement
slug: bureau-of-safety-and-environmental-enforcement-domain-security
source_filename: bureau-of-safety-and-environmental-enforcement-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bsee.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 21:44:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.data.bsee.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: timsweb.bsee.gov\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bsee.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bureau-of-safety-and-environmental-enforcement/refs/heads/main/security/bureau-of-safety-and-environmental-enforcement-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Enforcement
- Environment
- Federal Government
- Safety
- Offshore
- Oil and Gas
- Wells
---
