---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: moss.land
  spf: true
hosts:
- cert_expires: Oct  3 06:21:27 2026 GMT
  host: alpha.moss.land
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alpha Mossland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alpha (Mossland), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Alpha (Mossland)
provider_slug: alpha-mossland
slug: alpha-mossland-domain-security
source_filename: alpha-mossland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: alpha.moss.land\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 06:21:27 2026 GMT\n  hsts: false\ndomains:\n- domain: moss.land\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpha-mossland/refs/heads/main/security/alpha-mossland-domain-security.yml
summary_line: TLSv1.3
tags:
- Cryptocurrency
- Public APIs
---
