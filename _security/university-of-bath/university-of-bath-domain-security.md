---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bath.ac.uk
  spf: true
hosts:
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: www.bath.ac.uk
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 20:01:40 2026 GMT
  host: purehost.bath.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: researchdata.bath.ac.uk
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Bath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Bath, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Bath
provider_slug: university-of-bath
slug: university-of-bath-domain-security
source_filename: university-of-bath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bath.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: false\n- host: purehost.bath.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 20:01:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: researchdata.bath.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bath.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-bath/refs/heads/main/security/university-of-bath-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- United Kingdom
- Research
- Open Data
- Library
- Metadata
---
