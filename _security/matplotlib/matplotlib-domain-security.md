---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: matplotlib.org
  spf: true
hosts:
- cert_expires: Oct  1 20:26:07 2026 GMT
  host: matplotlib.org
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Matplotlib Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Matplotlib, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Matplotlib
provider_slug: matplotlib
slug: matplotlib-domain-security
source_filename: matplotlib-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: matplotlib.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 20:26:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: matplotlib.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/matplotlib/refs/heads/main/security/matplotlib-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Charts
- Data Science
- Open Source
- Plotting
- Python
- Scientific Computing
- Visualization
---
