---
description: ''
domains:
- caa:
  - merbridge.github.io.
  - 0 issuewild "sectigo.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  dmarc: false
  dnssec: true
  domain: merbridge.io
  spf: false
hosts:
- cert_expires: Sep 20 11:52:53 2026 GMT
  host: merbridge.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Merbridge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Merbridge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Merbridge
provider_slug: merbridge
slug: merbridge-domain-security
source_filename: merbridge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: merbridge.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 11:52:53 2026 GMT\n  hsts: false\ndomains:\n- domain: merbridge.io\n  dnssec: true\n  caa:\n  - merbridge.github.io.\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/merbridge/refs/heads/main/security/merbridge-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- CNCF
- eBPF
- Networking
- Performance
- Service Mesh
---
