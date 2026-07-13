---
api_specs:
- filename: docs
  format: yaml
  label: IPregistry IP Geolocation and Threat Intelligence API
  slug: ipregistry-ip-geolocation-and-threat-intelligence-api
  spec_type: OpenAPI
  url: https://ipregistry.co/docs
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
  dmarc_policy: reject
  dnssec: true
  domain: ipregistry.co
  spf: true
hosts:
- cert_expires: Sep 14 13:55:36 2026 GMT
  host: ipregistry.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 02:11:48 2026 GMT
  host: api.ipregistry.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ipregistry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPregistry, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: IPregistry
provider_slug: ipregistry
slug: ipregistry-domain-security
source_filename: ipregistry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ipregistry.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:55:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.ipregistry.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 02:11:48 2026 GMT\n  hsts: null\ndomains:\n- domain: ipregistry.co\n  dnssec: true\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipregistry/refs/heads/main/security/ipregistry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- IP Geolocation
- Threat Intelligence
- IP Address
- ASN
- Carrier
- Security
- Location Data
- User-Agent Parsing
- VPN Detection
- Proxy Detection
---
