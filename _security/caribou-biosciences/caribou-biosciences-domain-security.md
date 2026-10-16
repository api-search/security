---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: cariboubio.com
  spf: true
hosts:
- cert_expires: Dec 30 23:58:57 2026 GMT
  host: www.cariboubio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Caribou Biosciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caribou Biosciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Caribou Biosciences
provider_slug: caribou-biosciences
slug: caribou-biosciences-domain-security
source_filename: caribou-biosciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cariboubio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:58:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cariboubio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caribou-biosciences/refs/heads/main/security/caribou-biosciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Biotechnology
- Genome Editing
- Cell Therapy
- CRISPR
---
