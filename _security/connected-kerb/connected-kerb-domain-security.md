---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: connectedkerb.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.connectedkerb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: cp.connectedkerb.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Connected Kerb Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connected Kerb, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Connected Kerb
provider_slug: connected-kerb
slug: connected-kerb-domain-security
source_filename: connected-kerb-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.connectedkerb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\n- host: cp.connectedkerb.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: connectedkerb.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connected-kerb/refs/heads/main/security/connected-kerb-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- EV Charging
- Electric Vehicles
- Charge Point Operator
- Energy
- Transportation
- Smart Charging
- OCPI
- Roaming
- United Kingdom
- Infrastructure
- Sustainability
---
