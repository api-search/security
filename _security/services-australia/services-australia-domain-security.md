---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: servicesaustralia.gov.au
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.servicesaustralia.gov.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Services Australia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Services Australia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Services Australia
provider_slug: services-australia
slug: services-australia-domain-security
source_filename: services-australia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.servicesaustralia.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: servicesaustralia.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/services-australia/refs/heads/main/security/services-australia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Government
- Australia
- Healthcare
- Medicare
- Social Services
- Claiming
- Web Services
---
