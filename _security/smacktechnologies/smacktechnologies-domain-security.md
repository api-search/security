---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smacktechnologies.com
  spf: true
hosts:
- cert_expires: Sep  3 09:26:41 2026 GMT
  host: smacktechnologies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smacktechnologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smacktechnologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Smacktechnologies
provider_slug: smacktechnologies
slug: smacktechnologies-domain-security
source_filename: smacktechnologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smacktechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:26:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: smacktechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smacktechnologies/refs/heads/main/security/smacktechnologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Defense
- National Security
- Machine Learning
- Autonomous Systems
- Government
---
