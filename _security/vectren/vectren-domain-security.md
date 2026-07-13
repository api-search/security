---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: centerpointenergy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vectren.com
  spf: true
hosts:
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.centerpointenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: vectren.com
  https: false
- host: builder.vectren.com
  https: false
kind: domain-security
layout: security
method: probed
name: Vectren Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vectren (CenterPoint Energy), probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vectren (CenterPoint Energy)
provider_slug: vectren
slug: vectren-domain-security
source_filename: vectren-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.centerpointenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: vectren.com\n  https: false\n- host: builder.vectren.com\n  https: false\ndomains:\n- domain: centerpointenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: vectren.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectren/refs/heads/main/security/vectren-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Electric Utility
- Energy
- Natural Gas
- Regulated Utility
- Utility
---
