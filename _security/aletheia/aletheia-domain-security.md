---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aletheiaapi.com
  spf: false
hosts:
- cert_expires: Oct  3 08:23:49 2026 GMT
  host: aletheiaapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aletheia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aletheia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Aletheia
provider_slug: aletheia
slug: aletheia-domain-security
source_filename: aletheia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aletheiaapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:23:49 2026 GMT\n  hsts: false\ndomains:\n- domain: aletheiaapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aletheia/refs/heads/main/security/aletheia-domain-security.yml
summary_line: TLSv1.3
tags:
- Finance
- Public APIs
---
