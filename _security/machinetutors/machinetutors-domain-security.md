---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: machinetutors.com
  spf: true
hosts:
- cert_expires: Sep 11 03:32:43 2026 GMT
  host: www.machinetutors.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Machinetutors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Machinetutors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Machinetutors
provider_slug: machinetutors
slug: machinetutors-domain-security
source_filename: machinetutors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.machinetutors.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 03:32:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: machinetutors.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/machinetutors/refs/heads/main/security/machinetutors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Machine Learning
- Public APIs
---
