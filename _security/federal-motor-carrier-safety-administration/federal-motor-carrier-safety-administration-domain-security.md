---
api_specs:
- filename: federal-motor-carrier-safety-administration-openapi.yml
  format: yaml
  label: Federal Motor Carrier Safety Administration QCMobile API
  slug: federal-motor-carrier-safety-administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-motor-carrier-safety-administration/refs/heads/main/openapi/federal-motor-carrier-safety-administration-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dot.gov
  spf: true
hosts:
- cert_expires: Jul 21 23:59:59 2026 GMT
  host: www.fmcsa.dot.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: mobile.fmcsa.dot.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Federal Motor Carrier Safety Administration Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Federal Motor Carrier Safety Administration, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Federal Motor Carrier Safety Administration
provider_slug: federal-motor-carrier-safety-administration
slug: federal-motor-carrier-safety-administration-domain-security
source_filename: federal-motor-carrier-safety-administration-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fmcsa.dot.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 21 23:59:59 2026 GMT\n  hsts: null\n- host: mobile.fmcsa.dot.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dot.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-motor-carrier-safety-administration/refs/heads/main/security/federal-motor-carrier-safety-administration-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Federal Government
- Safety
- Transportation
---
