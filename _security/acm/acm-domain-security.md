---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: acm.org
  spf: true
hosts:
- cert_expires: Sep  2 23:52:47 2026 GMT
  host: dl.acm.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 09:07:48 2026 GMT
  host: libraries.acm.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACM Digital Library, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: ACM Digital Library
provider_slug: acm
slug: acm-domain-security
source_filename: acm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dl.acm.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 23:52:47 2026 GMT\n  hsts: null\n- host: libraries.acm.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 09:07:48 2026 GMT\n  hsts: null\ndomains:\n- domain: acm.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acm/refs/heads/main/security/acm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Academic
- Bibliographic Records
- Citations
- Computing
- Conference Proceedings
- DOI
- Digital Library
- Journals
- Metadata
- Open Access
- Publications
- Research
- Scholarly
---
