---
api_specs:
- filename: v2
  format: yaml
  label: Tailscale REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://api.tailscale.com/api/v2
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tailscale.com
  spf: true
hosts:
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: tailscale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  2 06:41:16 2026 GMT
  host: api.tailscale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tailscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tailscale, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tailscale
provider_slug: tailscale
slug: tailscale-domain-security
source_filename: tailscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tailscale.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.tailscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 06:41:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tailscale.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tailscale/refs/heads/main/security/tailscale-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- VPN
- Mesh Networking
- WireGuard
- Zero Trust
- Networking
- Identity
---
