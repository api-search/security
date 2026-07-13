---
api_specs:
- filename: smartproxy-openapi.yml
  format: yaml
  label: Smartproxy Account Management API
  slug: proxy-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smartproxy/refs/heads/main/openapi/smartproxy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: smartproxy.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: decodo.com
  spf: true
hosts:
- cert_expires: Aug 25 09:25:06 2026 GMT
  host: smartproxy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 12:14:15 2026 GMT
  host: api.decodo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smartproxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smartproxy, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Smartproxy
provider_slug: smartproxy
slug: smartproxy-domain-security
source_filename: smartproxy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smartproxy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 09:25:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.decodo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 12:14:15 2026 GMT\n  hsts: null\ndomains:\n- domain: smartproxy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: decodo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smartproxy/refs/heads/main/security/smartproxy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Proxies
- Web Scraping
- Data Collection
- Residential Proxies
- Datacenter Proxies
- Mobile Proxies
- Network Infrastructure
---
