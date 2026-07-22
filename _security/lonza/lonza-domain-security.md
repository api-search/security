---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lonza.com
  spf: true
hosts:
- cert_expires: Aug 20 22:24:06 2026 GMT
  host: lonza.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lonza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lonza, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lonza
provider_slug: lonza
slug: lonza-domain-security
source_filename: lonza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lonza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 20 22:24:06 2026 GMT\n  hsts: null\ndomains:\n- domain: lonza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lonza/refs/heads/main/security/lonza-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Pharmaceutical
- Biotech
- CDMO
- Manufacturing
- Life Sciences
- Healthcare
---
