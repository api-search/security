---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ncd.gov
  spf: true
hosts:
- cert_expires: Oct  6 19:21:21 2026 GMT
  host: www.ncd.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Council On Disability Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Council on Disability, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Council on Disability
provider_slug: national-council-on-disability
slug: national-council-on-disability-domain-security
source_filename: national-council-on-disability-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncd.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 19:21:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ncd.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-council-on-disability/refs/heads/main/security/national-council-on-disability-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Disability
- Federal Government
- Policy
- Civil Rights
- Healthcare
- Independent Agency
---
