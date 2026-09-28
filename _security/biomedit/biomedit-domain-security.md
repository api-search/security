---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: biomedit.com
  spf: true
hosts:
- cert_expires: Nov 25 11:18:49 2026 GMT
  host: biomedit.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biomedit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BiomEdit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BiomEdit
provider_slug: biomedit
slug: biomedit-domain-security
source_filename: biomedit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: biomedit.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 11:18:49 2026 GMT\n  hsts: null\ndomains:\n- domain: biomedit.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biomedit/refs/heads/main/security/biomedit-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Animal Health
- Microbiome
- Biotechnology
- Innovation
---
