---
api_specs:
- filename: routeros-bridge-api-openapi.yml
  format: yaml
  label: RouterOS Bridge API
  slug: routeros-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-bridge-api-openapi.yml
- filename: routeros-dhcp-api-openapi.yml
  format: yaml
  label: RouterOS DHCP API
  slug: routeros-dhcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-dhcp-api-openapi.yml
- filename: routeros-dns-api-openapi.yml
  format: yaml
  label: RouterOS DNS API
  slug: routeros-dns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-dns-api-openapi.yml
- filename: routeros-firewall-api-openapi.yml
  format: yaml
  label: RouterOS Firewall API
  slug: routeros-firewall-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-firewall-api-openapi.yml
- filename: routeros-interface-api-openapi.yml
  format: yaml
  label: RouterOS Interface API
  slug: routeros-interface-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-interface-api-openapi.yml
- filename: routeros-ip-address-api-openapi.yml
  format: yaml
  label: RouterOS IP Address API
  slug: routeros-ip-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-ip-address-api-openapi.yml
- filename: routeros-routing-api-openapi.yml
  format: yaml
  label: RouterOS Routing API
  slug: routeros-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-routing-api-openapi.yml
- filename: routeros-system-api-openapi.yml
  format: yaml
  label: RouterOS System API
  slug: routeros-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-system-api-openapi.yml
- filename: routeros-vpn-api-openapi.yml
  format: yaml
  label: RouterOS VPN API
  slug: routeros-vpn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-vpn-api-openapi.yml
- filename: routeros-wireless-api-openapi.yml
  format: yaml
  label: RouterOS Wireless API
  slug: routeros-wireless-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/openapi/routeros-wireless-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mikrotik.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: mikrotik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 26 04:09:31 2026 GMT
  host: help.mikrotik.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Routeros Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RouterOS, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RouterOS
provider_slug: routeros
slug: routeros-domain-security
source_filename: routeros-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mikrotik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: help.mikrotik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 26 04:09:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mikrotik.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/routeros/refs/heads/main/security/routeros-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Networking
- Router
- Network Management
- Firewall
- MikroTik
---
