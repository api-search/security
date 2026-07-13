---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: caltech.edu
  spf: true
hosts:
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: www.caltech.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 19:09:35 2026 GMT
  host: data.caltech.edu
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: irsa.ipac.caltech.edu
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caltech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for California Institute of Technology, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: California Institute of Technology
provider_slug: caltech
slug: caltech-domain-security
source_filename: caltech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caltech.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\n- host: data.caltech.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:09:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: irsa.ipac.caltech.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: caltech.edu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caltech/refs/heads/main/security/caltech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Astronomy
- Open Data
- United States
---
