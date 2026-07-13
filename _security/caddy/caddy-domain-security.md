---
api_specs:
- filename: caddy-openapi.yml
  format: yaml
  label: Caddy Web Server
  slug: caddy-web-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caddy/refs/heads/main/openapi/caddy-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: caddyserver.com
  spf: true
hosts:
- cert_expires: Sep 12 13:44:27 2026 GMT
  host: caddyserver.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caddy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caddy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Caddy
provider_slug: caddy
slug: caddy-domain-security
source_filename: caddy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caddyserver.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 13:44:27 2026 GMT\n  hsts: false\ndomains:\n- domain: caddyserver.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caddy/refs/heads/main/security/caddy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automatic HTTPS
- Go
- Load Balancer
- Reverse Proxy
- TLS
- Web Server
---
