---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: tankerkoenig.de
  spf: true
hosts:
- cert_expires: Oct  4 00:24:42 2026 GMT
  host: creativecommons.tankerkoenig.de
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tankerkoenig Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tankerkoenig, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Tankerkoenig
provider_slug: tankerkoenig
slug: tankerkoenig-domain-security
source_filename: tankerkoenig-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: creativecommons.tankerkoenig.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  4 00:24:42 2026 GMT\n  hsts: false\ndomains:\n- domain: tankerkoenig.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tankerkoenig/refs/heads/main/security/tankerkoenig-domain-security.yml
summary_line: TLSv1.2
tags:
- Transportation
- Public APIs
---
