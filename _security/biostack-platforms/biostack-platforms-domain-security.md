---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getbiostack.com
  spf: false
hosts:
- cert_expires: Oct  3 12:52:24 2026 GMT
  host: www.getbiostack.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Biostack Platforms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Biostack Platforms, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Biostack Platforms
provider_slug: biostack-platforms
slug: biostack-platforms-domain-security
source_filename: biostack-platforms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getbiostack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:52:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: getbiostack.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biostack-platforms/refs/heads/main/security/biostack-platforms-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Healthcare
- Artificial Intelligence
- Machine Learning
- Data
- Life Sciences
- Drug Discovery
---
