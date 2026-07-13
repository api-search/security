---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: liverpool.ac.uk
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.liverpool.ac.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: livrepository.liverpool.ac.uk
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: datacat.liverpool.ac.uk
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: University Of Liverpool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Liverpool, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Liverpool
provider_slug: university-of-liverpool
slug: university-of-liverpool-domain-security
source_filename: university-of-liverpool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.liverpool.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: livrepository.liverpool.ac.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\n- host: datacat.liverpool.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: liverpool.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-liverpool/refs/heads/main/security/university-of-liverpool-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Repository
- OAI-PMH
- United Kingdom
---
