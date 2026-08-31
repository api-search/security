---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mutualofomaha.com
  spf: true
hosts:
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: www.mutualofomaha.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 08:46:10 2026 GMT
  host: view.mutualofomaha.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mutual Of Omaha Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mutual of Omaha, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mutual of Omaha
provider_slug: mutual-of-omaha-insurance
slug: mutual-of-omaha-insurance-domain-security
source_filename: mutual-of-omaha-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mutualofomaha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: view.mutualofomaha.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 08:46:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mutualofomaha.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mutual-of-omaha-insurance/refs/heads/main/security/mutual-of-omaha-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Life Insurance
- Medicare
- Employee Benefits
- Benefits Administration
- Group Insurance
- Financial Services
- Annuities
- Disability Insurance
- Dental Insurance
---
