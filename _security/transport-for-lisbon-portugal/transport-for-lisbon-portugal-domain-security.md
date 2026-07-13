---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: city-platform.com
  spf: false
hosts:
- cert_expires: Dec  5 16:02:27 2026 GMT
  host: emel.city-platform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Transport For Lisbon Portugal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transport for Lisbon, Portugal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Transport for Lisbon, Portugal
provider_slug: transport-for-lisbon-portugal
slug: transport-for-lisbon-portugal-domain-security
source_filename: transport-for-lisbon-portugal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: emel.city-platform.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  5 16:02:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: city-platform.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transport-for-lisbon-portugal/refs/heads/main/security/transport-for-lisbon-portugal-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Transportation
- Public APIs
---
