---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: giveffect.com
  spf: true
hosts:
- cert_expires: Sep  9 23:12:35 2026 GMT
  host: www.giveffect.com
  hsts: true
  hsts_max_age: 315360000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  9 23:12:35 2026 GMT
  host: api.giveffect.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Giveffect Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Giveffect, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Giveffect
provider_slug: giveffect
slug: giveffect-domain-security
source_filename: giveffect-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.giveffect.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 23:12:35 2026 GMT\n  hsts: true\n  hsts_max_age: 315360000\n- host: api.giveffect.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 23:12:35 2026 GMT\n  hsts: false\ndomains:\n- domain: giveffect.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/giveffect/refs/heads/main/security/giveffect-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Nonprofit
- Fundraising
- CRM
- Donations
- Volunteer Management
- Marketing Automation
- SaaS
---
