---
api_specs:
- filename: zerotier-controller-api-openapi.yml
  format: yaml
  label: ZeroTier controller API
  slug: zerotier-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-controller-api-openapi.yml
- filename: zerotier-network-api-openapi.yml
  format: yaml
  label: ZeroTier network API
  slug: zerotier-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-network-api-openapi.yml
- filename: zerotier-network-member-api-openapi.yml
  format: yaml
  label: ZeroTier network-member API
  slug: zerotier-network-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-network-member-api-openapi.yml
- filename: zerotier-organizations-api-openapi.yml
  format: yaml
  label: ZeroTier organizations API
  slug: zerotier-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-organizations-api-openapi.yml
- filename: zerotier-peer-api-openapi.yml
  format: yaml
  label: ZeroTier peer API
  slug: zerotier-peer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-peer-api-openapi.yml
- filename: zerotier-status-api-openapi.yml
  format: yaml
  label: ZeroTier status API
  slug: zerotier-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-status-api-openapi.yml
- filename: zerotier-user-api-openapi.yml
  format: yaml
  label: ZeroTier user API
  slug: zerotier-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-user-api-openapi.yml
- filename: zerotier-util-api-openapi.yml
  format: yaml
  label: ZeroTier util API
  slug: zerotier-util-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/openapi/zerotier-util-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: zerotier.com
  spf: true
hosts:
- cert_expires: Sep 21 03:04:13 2026 GMT
  host: www.zerotier.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 15:38:51 2026 GMT
  host: docs.zerotier.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 16:00:55 2026 GMT
  host: api.zerotier.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zerotier Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ZeroTier, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: ZeroTier
provider_slug: zerotier
slug: zerotier-domain-security
source_filename: zerotier-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zerotier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 03:04:13 2026 GMT\n  hsts: false\n- host: docs.zerotier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 15:38:51 2026 GMT\n  hsts: false\n- host: api.zerotier.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 16:00:55 2026 GMT\n  hsts: null\ndomains:\n- domain: zerotier.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zerotier/refs/heads/main/security/zerotier-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Networking
- Software-Defined Networking
- SDN
- VPN
- Security
- Connectivity
- Overlay Network
- Zero Trust
- Infrastructure
---
