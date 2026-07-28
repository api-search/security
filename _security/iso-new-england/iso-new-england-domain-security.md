---
api_specs:
- filename: iso-new-england-web-services-openapi.yml
  format: yaml
  label: ISO New England Web Services API v1.1
  slug: iso-ne-web-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/iso-new-england/refs/heads/main/openapi/iso-new-england-web-services-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iso-ne.com
  spf: true
hosts:
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: www.iso-ne.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 23:59:59 2026 GMT
  host: webservices.iso-ne.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iso New England Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ISO New England, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ISO New England
provider_slug: iso-new-england
slug: iso-new-england-domain-security
source_filename: iso-new-england-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.iso-ne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: webservices.iso-ne.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iso-ne.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iso-new-england/refs/heads/main/security/iso-new-england-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- United States
- Electricity
- Energy Markets
- Grid
- Open Data
- Wholesale Markets
- Demand Response
- Renewables
- New England
---
