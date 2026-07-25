---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nbc.ca
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flinks.com
  spf: true
hosts:
- cert_expires: Dec  7 09:05:22 2026 GMT
  host: www.nbc.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  2 18:00:01 2026 GMT
  host: www.flinks.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: National Bank Of Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for National Bank of Canada, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: National Bank of Canada
provider_slug: national-bank-of-canada
slug: national-bank-of-canada-domain-security
source_filename: national-bank-of-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nbc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 09:05:22 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.flinks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 18:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: nbc.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: flinks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-bank-of-canada/refs/heads/main/security/national-bank-of-canada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Banking
- Canada
- Big Six
- Open Banking
- Consumer-Driven Banking
- FDX
- Data Aggregation
- Payments
---
