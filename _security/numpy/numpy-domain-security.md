---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: numpy.org
  spf: true
hosts:
- cert_expires: Sep  8 18:30:15 2026 GMT
  host: numpy.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Numpy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NumPy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NumPy
provider_slug: numpy
slug: numpy-domain-security
source_filename: numpy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numpy.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 18:30:15 2026 GMT\n  hsts: false\ndomains:\n- domain: numpy.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numpy/refs/heads/main/security/numpy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Data Science
- Machine Learning
- Numerical Analysis
- Open Source
- Python Library
- Scientific Computing
---
