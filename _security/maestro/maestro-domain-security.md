---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: maestropms.com
  spf: true
hosts:
- cert_expires: Sep 24 15:57:40 2026 GMT
  host: maestropms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maestro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maestro PMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Maestro PMS
provider_slug: maestro
slug: maestro-domain-security
source_filename: maestro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maestropms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 15:57:40 2026 GMT\n  hsts: false\ndomains:\n- domain: maestropms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maestro/refs/heads/main/security/maestro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Property Management
- Hospitality
- Hotels
- PMS
- Resorts
---
