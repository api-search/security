---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: storyraise.com
  spf: true
hosts:
- cert_expires: Jan 24 20:13:10 2027 GMT
  host: storyraise.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Storyraise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Storyraise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Storyraise
provider_slug: storyraise
slug: storyraise-domain-security
source_filename: storyraise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: storyraise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 20:13:10 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: storyraise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/storyraise/security/storyraise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Nonprofit
- Fundraising
- DonorManagement
- SaaS
---
