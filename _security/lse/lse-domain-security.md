---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lse.ac.uk
  spf: true
hosts:
- cert_expires: Aug 15 23:59:59 2026 GMT
  host: www.lse.ac.uk
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 27 09:46:53 2026 GMT
  host: researchonline.lse.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  5 23:59:59 2027 GMT
  host: digital.library.lse.ac.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for London School of Economics and Political Science, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: London School of Economics and Political Science
provider_slug: lse
slug: lse-domain-security
source_filename: lse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lse.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: researchonline.lse.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 09:46:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: digital.library.lse.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lse.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lse/refs/heads/main/security/lse-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Library
- Open Research
- Repository
- OAI-PMH
- IIIF
- Identity
---
