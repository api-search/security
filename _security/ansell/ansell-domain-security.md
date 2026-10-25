---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ansell.com
  spf: true
hosts:
- cert_expires: Jan 19 15:21:44 2027 GMT
  host: www.ansell.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ansell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ansell, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ansell
provider_slug: ansell
slug: ansell-domain-security
source_filename: ansell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ansell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 15:21:44 2027 GMT\n  hsts: null\ndomains:\n- domain: ansell.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansell/refs/heads/main/security/ansell-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Personal Protective Equipment
- Gloves
- Healthcare
- Manufacturing
- Industrial Safety
- Australia
---
