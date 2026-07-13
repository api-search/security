---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aishub.net
  spf: true
hosts:
- cert_expires: Aug 31 20:33:05 2026 GMT
  host: www.aishub.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ais Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIS Hub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: AIS Hub
provider_slug: ais-hub
slug: ais-hub-domain-security
source_filename: ais-hub-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aishub.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 20:33:05 2026 GMT\n  hsts: false\ndomains:\n- domain: aishub.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ais-hub/refs/heads/main/security/ais-hub-domain-security.yml
summary_line: TLSv1.3
tags:
- Transportation
- Public APIs
---
