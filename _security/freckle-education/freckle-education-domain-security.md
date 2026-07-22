---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: freckle.com
  spf: true
hosts:
- cert_expires: Sep 14 07:13:40 2026 GMT
  host: freckle.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freckle Education Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freckle Education, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Freckle Education
provider_slug: freckle-education
slug: freckle-education-domain-security
source_filename: freckle-education-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: freckle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 07:13:40 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: freckle.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freckle-education/refs/heads/main/security/freckle-education-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Education
- EdTech
- K-12
- Adaptive Learning
- Mathematics
- English Language Arts
- Renaissance
---
