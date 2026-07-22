---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: urbanlogiq.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: urbanlogiq.us
  spf: false
hosts:
- cert_expires: Oct 18 05:35:27 2026 GMT
  host: urbanlogiq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 07:11:39 2026 GMT
  host: home.urbanlogiq.us
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urbanlogiq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UrbanLogiq, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UrbanLogiq
provider_slug: urbanlogiq
slug: urbanlogiq-domain-security
source_filename: urbanlogiq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urbanlogiq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 05:35:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: home.urbanlogiq.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 07:11:39 2026 GMT\n  hsts: null\ndomains:\n- domain: urbanlogiq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: urbanlogiq.us\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanlogiq/refs/heads/main/security/urbanlogiq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government
- GovTech
- Data
- Analytics
- Transportation
- Urban Planning
- Public Safety
- Economic Development
- Artificial Intelligence
---
