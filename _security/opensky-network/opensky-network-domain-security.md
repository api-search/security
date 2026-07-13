---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opensky-network.org
  spf: true
hosts:
- cert_expires: Sep  4 10:59:22 2026 GMT
  host: opensky-network.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opensky Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenSky Network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: OpenSky Network
provider_slug: opensky-network
slug: opensky-network-domain-security
source_filename: opensky-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opensky-network.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 10:59:22 2026 GMT\n  hsts: null\ndomains:\n- domain: opensky-network.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opensky-network/refs/heads/main/security/opensky-network-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Transportation
- Public APIs
---
