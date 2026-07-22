---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gireve.com
  spf: true
hosts:
- cert_expires: Aug 26 02:08:45 2026 GMT
  host: www.gireve.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gireve Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gireve, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Gireve
provider_slug: gireve
slug: gireve-domain-security
source_filename: gireve-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gireve.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 02:08:45 2026 GMT\n  hsts: false\ndomains:\n- domain: gireve.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gireve/refs/heads/main/security/gireve-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate
- Electric Vehicles
- EV Charging
- Roaming
- Interoperability
- Mobility
- OCPI
- Energy
---
