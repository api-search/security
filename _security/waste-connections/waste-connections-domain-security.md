---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wasteconnections.com
  spf: true
hosts:
- cert_expires: Sep  7 00:00:01 2026 GMT
  host: www.wasteconnections.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 06:44:20 2026 GMT
  host: myaccount.wasteconnections.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Waste Connections Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Waste Connections, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Waste Connections
provider_slug: waste-connections
slug: waste-connections-domain-security
source_filename: waste-connections-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wasteconnections.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 00:00:01 2026 GMT\n  hsts: null\n- host: myaccount.wasteconnections.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 06:44:20 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: wasteconnections.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waste-connections/refs/heads/main/security/waste-connections-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Environmental Services
- Fortune 500
- Recycling
- Solid Waste
- Sustainability
- Waste Management
---
