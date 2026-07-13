---
api_specs:
- filename: digital-ocean-openapi-original.yml
  format: yaml
  label: Digital Ocean API
  slug: digital-ocean-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digital-ocean/refs/heads/main/openapi/digital-ocean-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: digitalocean.com
  spf: true
hosts:
- cert_expires: Sep 25 14:26:22 2026 GMT
  host: docs.digitalocean.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 14:26:22 2026 GMT
  host: api.digitalocean.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Digital Ocean Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Digital Ocean, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Digital Ocean
provider_slug: digital-ocean
slug: digital-ocean-domain-security
source_filename: digital-ocean-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.digitalocean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:26:22 2026 GMT\n  hsts: false\n- host: api.digitalocean.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 14:26:22 2026 GMT\n  hsts: false\ndomains:\n- domain: digitalocean.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digital-ocean/refs/heads/main/security/digital-ocean-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Cloud
- Compute
- Servers
- Infrastructure
---
