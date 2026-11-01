---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: medigami.com
  spf: true
hosts:
- cert_expires: Dec 20 10:12:26 2026 GMT
  host: medigami.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Medigami Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for medigami-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: medigami-com
provider_slug: medigami-com
slug: medigami-com-domain-security
source_filename: medigami-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: medigami.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 10:12:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: medigami.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/medigami-com/security/medigami-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- HealthTech
- Imaging
- DataAnalytics
- API
- Healthcare
---
