---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: arkocorp.com
  spf: true
hosts:
- cert_expires: Aug 26 08:03:47 2026 GMT
  host: www.arkocorp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Arko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ARKO Corp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ARKO Corp
provider_slug: arko
slug: arko-domain-security
source_filename: arko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.arkocorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 08:03:47 2026 GMT\n  hsts: false\ndomains:\n- domain: arkocorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arko/refs/heads/main/security/arko-domain-security.yml
summary_line: TLSv1.3
tags:
- Convenience Stores
- Fleet Fueling
- Fuel
- Petroleum
- Retail
---
