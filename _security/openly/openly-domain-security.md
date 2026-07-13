---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: openly.com
  spf: true
hosts:
- cert_expires: Sep 20 05:02:47 2026 GMT
  host: openly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 22:43:22 2026 GMT
  host: developers.openly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 16:32:56 2026 GMT
  host: api.openly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Openly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Openly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Openly
provider_slug: openly
slug: openly-domain-security
source_filename: openly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:02:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.openly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 22:43:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.openly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 16:32:56 2026 GMT\n  hsts: null\ndomains:\n- domain: openly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openly/refs/heads/main/security/openly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Homeowners Insurance
- Home Insurance
- Quote
- Bind
- Policy
- Endorsement
- Renewal
- InsurTech
---
