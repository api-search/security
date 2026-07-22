---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: svcreit.com
  spf: true
hosts:
- cert_expires: Aug 28 10:50:46 2026 GMT
  host: www.svcreit.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Service Properties Trust Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Service Properties Trust, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Service Properties Trust
provider_slug: service-properties-trust
slug: service-properties-trust-domain-security
source_filename: service-properties-trust-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.svcreit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 10:50:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: svcreit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/service-properties-trust/refs/heads/main/security/service-properties-trust-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real Estate
- REIT
- Hospitality
- Hotels
- Net Lease
- Retail
- Travel
- Lodging
- Investor Relations
- Fortune 1000
---
