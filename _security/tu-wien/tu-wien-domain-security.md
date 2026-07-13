---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tuwien.at
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tuwien.ac.at
  spf: true
hosts:
- cert_expires: Dec  6 11:58:26 2026 GMT
  host: www.tuwien.at
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 21:20:39 2026 GMT
  host: researchdata.tuwien.ac.at
  hsts: true
  hsts_max_age: 31556926
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 09:25:49 2026 GMT
  host: repositum.tuwien.at
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tu Wien Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TU Wien, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: TU Wien
provider_slug: tu-wien
slug: tu-wien-domain-security
source_filename: tu-wien-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tuwien.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 11:58:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: researchdata.tuwien.ac.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 21:20:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31556926\n- host: repositum.tuwien.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 09:25:49 2026 GMT\n  hsts: false\ndomains:\n- domain: tuwien.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: tuwien.ac.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tu-wien/refs/heads/main/security/tu-wien-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research Data
- Open Access
- Repository
- OAI-PMH
- InvenioRDM
- Austria
- Europe
---
