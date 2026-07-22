---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ornl.gov
  spf: true
hosts:
- cert_expires: Sep  9 18:02:22 2026 GMT
  host: www.ornl.gov
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oak Ridge National Laboratory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oak Ridge National Laboratory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Oak Ridge National Laboratory
provider_slug: oak-ridge-national-laboratory
slug: oak-ridge-national-laboratory-domain-security
source_filename: oak-ridge-national-laboratory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ornl.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 18:02:22 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: ornl.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oak-ridge-national-laboratory/refs/heads/main/security/oak-ridge-national-laboratory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- DOE
- Energy
- Government
- National Laboratory
- Research
- Science
---
