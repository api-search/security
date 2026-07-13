---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: leeds.ac.uk
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.leeds.ac.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 23:59:59 2026 GMT
  host: archive.researchdata.leeds.ac.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: library.leeds.ac.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Leeds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Leeds, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Leeds
provider_slug: university-of-leeds
slug: university-of-leeds-domain-security
source_filename: university-of-leeds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.leeds.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: archive.researchdata.leeds.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: library.leeds.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: leeds.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-leeds/refs/heads/main/security/university-of-leeds-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Research Data
- Libraries
- OAI-PMH
- IIIF
---
