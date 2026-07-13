---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unibo.it
  spf: true
hosts:
- cert_expires: Aug 18 09:14:49 2026 GMT
  host: www.unibo.it
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 18 09:14:49 2026 GMT
  host: dati.unibo.it
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 18 09:14:49 2026 GMT
  host: amsacta.unibo.it
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: University Of Bologna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Bologna, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Bologna
provider_slug: university-of-bologna
slug: university-of-bologna-domain-security
source_filename: university-of-bologna-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unibo.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 18 09:14:49 2026 GMT\n  hsts: false\n- host: dati.unibo.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 18 09:14:49 2026 GMT\n  hsts: false\n- host: amsacta.unibo.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 18 09:14:49 2026 GMT\n  hsts: false\ndomains:\n- domain: unibo.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-bologna/refs/heads/main/security/university-of-bologna-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Education
- Higher Education
- University
- Open Data
- Research
- Italy
- Europe
---
