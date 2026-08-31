---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: troymedicare.com
  spf: true
hosts:
- cert_expires: Nov 26 16:36:59 2026 GMT
  host: troymedicare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 16 06:07:24 2026 GMT
  host: provider.troymedicare.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 24 08:05:40 2026 GMT
  host: fhir.troymedicare.com
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Troy Medicare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Troy Medicare, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Troy Medicare
provider_slug: troy-medicare
slug: troy-medicare-domain-security
source_filename: troy-medicare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: troymedicare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 16:36:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: provider.troymedicare.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 16 06:07:24 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: fhir.troymedicare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 08:05:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\ndomains:\n- domain: troymedicare.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/troy-medicare/refs/heads/main/security/troy-medicare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Health Insurance
- Medicare
- Medicare Advantage
- Health Plans
- Healthcare
- Pharmacy
- Care Management
- Insurance
- Identity
- OpenID Connect
---
