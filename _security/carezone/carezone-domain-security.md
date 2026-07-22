---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carezone.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: carezone.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carezone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carezone, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Carezone
provider_slug: carezone
slug: carezone-domain-security
source_filename: carezone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carezone.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: carezone.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carezone/refs/heads/main/security/carezone-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Human Health
- Medication Management
- Digital Health
- Pharmacy
- Consumer Health
- Care Coordination
---
