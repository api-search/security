---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: enviri.com
  spf: true
hosts:
- cert_expires: Sep  8 17:04:17 2026 GMT
  host: www.enviri.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Harsco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enviri (formerly Harsco), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Enviri (formerly Harsco)
provider_slug: harsco
slug: harsco-domain-security
source_filename: harsco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enviri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 17:04:17 2026 GMT\n  hsts: false\ndomains:\n- domain: enviri.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harsco/refs/heads/main/security/harsco-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Environmental Services
- Hazardous Waste
- Industrial
- Rail
- Recycling
- Steel
- Sustainability
---
