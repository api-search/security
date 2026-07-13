---
api_specs:
- filename: ipinfo-openapi.yml
  format: yaml
  label: IPinfo Core API
  slug: ipinfo-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipinfo/main/openapi/ipinfo-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ipinfo.io
  spf: true
hosts:
- cert_expires: Sep 15 15:37:33 2026 GMT
  host: ipinfo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 15:37:33 2026 GMT
  host: api.ipinfo.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 15:37:33 2026 GMT
  host: v6.ipinfo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ipinfo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPinfo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IPinfo
provider_slug: ipinfo
slug: ipinfo-domain-security
source_filename: ipinfo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipinfo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:37:33 2026 GMT\n  hsts: false\n- host: api.ipinfo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:37:33 2026 GMT\n  hsts: null\n- host: v6.ipinfo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 15:37:33 2026 GMT\n  hsts: false\ndomains:\n- domain: ipinfo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipinfo/refs/heads/main/security/ipinfo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- IP Intelligence
- IP Geolocation
- ASN
- Privacy Detection
- VPN Detection
- Threat Intelligence
- Network Data
- Mobile Carrier
- WHOIS
- Public APIs
- Development
---
