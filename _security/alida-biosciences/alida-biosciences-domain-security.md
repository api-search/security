---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: alidabio.com
  spf: true
hosts:
- cert_expires: Dec 23 20:58:40 2026 GMT
  host: www.alidabio.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alida Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alida Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Alida Biosciences
provider_slug: alida-biosciences
slug: alida-biosciences-domain-security
source_filename: alida-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alidabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 20:58:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: alidabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alida-biosciences/refs/heads/main/security/alida-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Biotechnology
- RNA
- Epitranscriptomics
- San-Diego
---
