---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: conagen.com
  spf: true
hosts:
- cert_expires: Nov 25 09:03:14 2026 GMT
  host: conagen.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Conagen Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Conagen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Conagen
provider_slug: conagen
slug: conagen-domain-security
source_filename: conagen-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: conagen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 09:03:14 2026 GMT\n  hsts: false\ndomains:\n- domain: conagen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/conagen/refs/heads/main/security/conagen-domain-security.yml
summary_line: TLSv1.3
tags:
- Synthetic Biology
- Biomanufacturing
- Biotechnology
- Engineering
- Food Ingredients
---
