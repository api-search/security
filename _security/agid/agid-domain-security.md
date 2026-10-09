---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: agid.gov.it
  spf: true
hosts:
- cert_expires: Dec  1 16:14:41 2026 GMT
  host: www.agid.gov.it
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AgID (Agenzia per l''Italia Digitale), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AgID (Agenzia per l'Italia Digitale)
provider_slug: agid
slug: agid-domain-security
source_filename: agid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agid.gov.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 16:14:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agid.gov.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agid/refs/heads/main/security/agid-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Government
- Public Sector
- Italy
- Digital Transformation
- Guidelines
- Spectral
---
