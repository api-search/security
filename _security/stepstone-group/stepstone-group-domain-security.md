---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stepstonegroup.com
  spf: true
hosts:
- cert_expires: Sep 27 20:17:20 2026 GMT
  host: www.stepstonegroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: developer.stepstonegroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 23:59:59 2026 GMT
  host: api.stepstonegroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stepstone Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StepStone Group, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StepStone Group
provider_slug: stepstone-group
slug: stepstone-group-domain-security
source_filename: stepstone-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stepstonegroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 20:17:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.stepstonegroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stepstonegroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: stepstonegroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stepstone-group/refs/heads/main/security/stepstone-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Private Markets
- Investment
- Data
---
