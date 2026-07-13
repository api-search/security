---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:certificates@uq.edu.au"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uq.edu.au
  spf: true
hosts:
- cert_expires: Nov 24 23:59:59 2026 GMT
  host: www.uq.edu.au
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 23:59:59 2026 GMT
  host: espace.library.uq.edu.au
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 16 18:45:20 2026 GMT
  host: data.uq.edu.au
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Queensland, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: University of Queensland
provider_slug: uq
slug: uq-domain-security
source_filename: uq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.uq.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 23:59:59 2026 GMT\n  hsts: false\n- host: espace.library.uq.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 23:59:59 2026 GMT\n  hsts: null\n- host: data.uq.edu.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 18:45:20 2026 GMT\n  hsts: null\ndomains:\n- domain: uq.edu.au\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:certificates@uq.edu.au\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uq/refs/heads/main/security/uq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Education
- Higher Education
- University
- Research
- Library
- Institutional Repository
- Open Data
- Australia
---
