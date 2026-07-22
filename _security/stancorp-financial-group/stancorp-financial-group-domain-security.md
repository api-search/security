---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: standard.com
  spf: true
hosts:
- cert_expires: Sep 16 18:14:41 2026 GMT
  host: www.standard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stancorp Financial Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StanCorp Financial Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StanCorp Financial Group
provider_slug: stancorp-financial-group
slug: stancorp-financial-group-domain-security
source_filename: stancorp-financial-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.standard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 18:14:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: standard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stancorp-financial-group/refs/heads/main/security/stancorp-financial-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Benefits Administration
- Disability Insurance
- Employee Benefits
- Financial Services
- Insurance
- Life Insurance
- Retirement Plans
---
