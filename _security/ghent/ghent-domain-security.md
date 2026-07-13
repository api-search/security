---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ugent.be
  spf: true
hosts:
- cert_expires: Nov 13 04:16:24 2026 GMT
  host: www.ugent.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 08:19:39 2026 GMT
  host: biblio.ugent.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 13 01:01:17 2026 GMT
  host: lib.ugent.be
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ghent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ghent University, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ghent University
provider_slug: ghent
slug: ghent-domain-security
source_filename: ghent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ugent.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 04:16:24 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: biblio.ugent.be\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 14 08:19:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: lib.ugent.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 01:01:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ugent.be\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ghent/refs/heads/main/security/ghent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Open Data
- Belgium
- Europe
---
