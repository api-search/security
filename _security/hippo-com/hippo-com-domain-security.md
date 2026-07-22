---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hippo.com
  spf: true
hosts:
- cert_expires: Aug 10 15:17:31 2026 GMT
  host: www.hippo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hippo Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hippo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hippo
provider_slug: hippo-com
slug: hippo-com-domain-security
source_filename: hippo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hippo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 15:17:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hippo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hippo-com/refs/heads/main/security/hippo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Home Insurance
- Homeowners Insurance
- Smart Home
- Insurtech
- Property Insurance
- Condo Insurance
- Landlord Insurance
- Flood Insurance
- MGA
- Carrier
- Claims
- Underwriting
- Mobile App
- Consumer
---
