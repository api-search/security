---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: genomatica.com
  spf: true
hosts:
- cert_expires: Sep  5 23:25:01 2026 GMT
  host: www.genomatica.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Genomatica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Genomatica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Genomatica
provider_slug: genomatica
slug: genomatica-domain-security
source_filename: genomatica-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.genomatica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:25:01 2026 GMT\n  hsts: null\ndomains:\n- domain: genomatica.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genomatica/refs/heads/main/security/genomatica-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Sustainability
- Materials
- Chemicals
- Manufacturing
- Renewable
- Industrial Biotech
---
