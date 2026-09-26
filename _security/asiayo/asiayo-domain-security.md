---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: asiayo.com
  spf: true
hosts:
- cert_expires: Mar 27 21:48:31 2027 GMT
  host: asiayo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asiayo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asiayo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Asiayo
provider_slug: asiayo
slug: asiayo-domain-security
source_filename: asiayo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asiayo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 27 21:48:31 2027 GMT\n  hsts: null\ndomains:\n- domain: asiayo.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asiayo/refs/heads/main/security/asiayo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Marketplace
- Booking
- Tours
- Hospitality
---
