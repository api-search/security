---
api_specs:
- filename: ipify-ip-api.yml
  format: yaml
  label: ipify Public IP Address API
  slug: ipify-public-ip-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipify/refs/heads/main/openapi/ipify-ip-api.yml
- filename: ipify-geolocation-api.yml
  format: yaml
  label: ipify IP Geolocation API
  slug: ipify-ip-geolocation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipify/refs/heads/main/openapi/ipify-geolocation-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ipify.org
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.ipify.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 03:07:45 2026 GMT
  host: api.ipify.org
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 03:07:45 2026 GMT
  host: geo.ipify.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ipify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ipify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ipify
provider_slug: ipify
slug: ipify-domain-security
source_filename: ipify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ipify.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: false\n- host: api.ipify.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:07:45 2026 GMT\n  hsts: null\n- host: geo.ipify.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 03:07:45 2026 GMT\n  hsts: false\ndomains:\n- domain: ipify.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipify/refs/heads/main/security/ipify-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Development
- IP Address
- Geolocation
- IP Intelligence
- Public APIs
---
