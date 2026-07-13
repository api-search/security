---
api_specs:
- filename: national-institute-of-standards-and-technology-openapi.yml
  format: yaml
  label: NIST National Vulnerability Database (NVD) API
  slug: nvd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-institute-of-standards-and-technology/main/openapi/national-institute-of-standards-and-technology-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nist.gov
  spf: true
hosts:
- cert_expires: Sep 24 09:16:11 2026 GMT
  host: www.nist.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 12:26:14 2026 GMT
  host: nvd.nist.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 14:16:22 2026 GMT
  host: services.nvd.nist.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Institute Of Standards And Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Institute of Standards and Technology, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: National Institute of Standards and Technology
provider_slug: national-institute-of-standards-and-technology
slug: national-institute-of-standards-and-technology-domain-security
source_filename: national-institute-of-standards-and-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nist.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 09:16:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: nvd.nist.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:26:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services.nvd.nist.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 14:16:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nist.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-institute-of-standards-and-technology/refs/heads/main/security/national-institute-of-standards-and-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cybersecurity
- Federal Government
- Standards
- Technology
- Vulnerabilities
---
