---
api_specs:
- filename: frp-server-admin-api-openapi.yml
  format: yaml
  label: frp Server Admin API
  slug: server-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frp/refs/heads/main/openapi/frp-server-admin-api-openapi.yml
- filename: frp-client-admin-api-openapi.yml
  format: yaml
  label: frp Client Admin API
  slug: client-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/frp/refs/heads/main/openapi/frp-client-admin-api-openapi.yml
description: ''
domains:
- caa:
  - gofrp.github.io.
  - 0 issue "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  dmarc: false
  dnssec: true
  domain: gofrp.org
  spf: false
hosts:
- cert_expires: Sep 26 10:19:27 2026 GMT
  host: gofrp.org
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- host: 127.0.0.1
  https: false
kind: domain-security
layout: security
method: probed
name: Frp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for frp, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: frp
provider_slug: frp
slug: frp-domain-security
source_filename: frp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gofrp.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 10:19:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: 127.0.0.1\n  https: false\ndomains:\n- domain: gofrp.org\n  dnssec: true\n  caa:\n  - gofrp.github.io.\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/frp/refs/heads/main/security/frp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- NAT Traversal
- Reverse Proxy
- Tunneling
- Open Source
---
