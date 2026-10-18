---
api_specs:
- filename: igrant-io-config-api-openapi.yml
  format: yaml
  label: iGrant.io Config API
  slug: igrant-io-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/igrant-io/refs/heads/main/openapi/igrant-io-config-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: igrant.io
  spf: true
hosts:
- cert_expires: Dec 31 16:08:09 2026 GMT
  host: igrant.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Igrant Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iGrant.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: iGrant.io
provider_slug: igrant-io
slug: igrant-io-domain-security
source_filename: igrant-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: igrant.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 16:08:09 2026 GMT\n  hsts: false\ndomains:\n- domain: igrant.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/igrant-io/refs/heads/main/security/igrant-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Identity
- Wallets
- eIDAS
---
