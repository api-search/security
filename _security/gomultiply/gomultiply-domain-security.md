---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gomultiply.com
  spf: true
hosts:
- cert_expires: Aug 21 04:14:50 2026 GMT
  host: gomultiply.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gomultiply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gomultiply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gomultiply
provider_slug: gomultiply
slug: gomultiply-domain-security
source_filename: gomultiply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gomultiply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 04:14:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gomultiply.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gomultiply/refs/heads/main/security/gomultiply-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Marketing
- Artificial Intelligence
- B2B
- Paid Media
- Agency
- MarTech
- LinkedIn Ads
- Google Ads
---
