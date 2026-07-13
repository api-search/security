---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Rentvine REST API
  slug: rentvine-api
  spec_type: OpenAPI
  url: https://docs.rentvine.com/
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rentvine.com
  spf: true
hosts:
- cert_expires: Aug  6 14:17:52 2026 GMT
  host: www.rentvine.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: docs.rentvine.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rentvine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rentvine, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rentvine
provider_slug: rentvine
slug: rentvine-domain-security
source_filename: rentvine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rentvine.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug  6 14:17:52 2026 GMT\n  hsts: false\n- host: docs.rentvine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: rentvine.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rentvine/refs/heads/main/security/rentvine-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Property Management
- Real Estate
- Leasing
- Tenant Management
- Maintenance
- Trust Accounting
- Owner Portals
- REST API
---
