---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: crowdtap.com
  spf: true
hosts:
- cert_expires: Dec 12 07:21:03 2026 GMT
  host: crowdtap.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crowdtap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crowdtap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Crowdtap
provider_slug: crowdtap
slug: crowdtap-domain-security
source_filename: crowdtap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: crowdtap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 07:21:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crowdtap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crowdtap/refs/heads/main/security/crowdtap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ConsumerRewards
- Surveys
- Market Research
- Mobile App
- Gift Cards
---
