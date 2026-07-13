---
api_specs:
- filename: vpn-openapi.yml
  format: yaml
  label: NordVPN API
  slug: nordvpn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vpn/refs/heads/main/openapi/vpn-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tailscale.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nordvpn.com
  spf: true
hosts:
- cert_expires: Mar 17 23:59:59 2027 GMT
  host: tailscale.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.nordvpn.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 13:13:16 2026 GMT
  host: protonvpn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vpn Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for VPN, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: VPN
provider_slug: vpn
slug: vpn-domain-security
source_filename: vpn-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tailscale.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 17 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.nordvpn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: protonvpn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 13:13:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tailscale.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nordvpn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vpn/refs/heads/main/security/vpn-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Encryption
- Networking
- Privacy
- Security
- VPN
---
