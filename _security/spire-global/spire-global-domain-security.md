---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: spire.com
  spf: true
hosts:
- cert_expires: Sep 14 00:11:44 2026 GMT
  host: spire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 08:52:42 2026 GMT
  host: documentation.spire.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.maritime.spire.com
  https: false
kind: domain-security
layout: security
method: probed
name: Spire Global Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spire Global, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Spire Global
provider_slug: spire-global
slug: spire-global-domain-security
source_filename: spire-global-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 00:11:44 2026 GMT\n  hsts: false\n- host: documentation.spire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:52:42 2026 GMT\n  hsts: false\n- host: api.maritime.spire.com\n  https: false\ndomains:\n- domain: spire.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spire-global/refs/heads/main/security/spire-global-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Satellites
- Earth Observation
- AIS
- Maritime
- ADS-B
- Aviation
- Weather
- RF Geolocation
- GraphQL
- LEMUR
- GNSS-RO
---
