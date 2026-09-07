---
api_specs:
- filename: beacon-roofing-supply-v2-openapi.yml
  format: yaml
  label: Beacon PRO+ API (V2, OAuth)
  slug: beacon-pro-plus
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-v2-openapi.yml
- filename: beacon-roofing-supply-all-api-openapi.yml
  format: yaml
  label: Beacon External Rest Service (all_api)
  slug: beacon-rest-all-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-all-api-openapi.yml
- filename: beacon-roofing-supply-v3-openapi.yml
  format: yaml
  label: Beacon Rest Services V3 (Public / Integrations)
  slug: beacon-rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-v3-openapi.yml
- filename: beacon-roofing-supply-v1-openapi.yml
  format: yaml
  label: Beacon Rest Services V1 (session)
  slug: beacon-rest-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-v1-openapi.yml
- filename: beacon-roofing-supply-oauth2-openapi.yml
  format: yaml
  label: Beacon OAuth Rest Service
  slug: beacon-oauth
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-oauth2-openapi.yml
- filename: beacon-roofing-supply-public-openapi.yml
  format: yaml
  label: Beacon Rest Services Public
  slug: beacon-rest-public
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-public-openapi.yml
- filename: beacon-roofing-supply-internal-openapi.yml
  format: yaml
  label: Beacon Internal Rest Service
  slug: beacon-rest-internal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/openapi/beacon-roofing-supply-internal-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: becn.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: beaconproplus.com
  spf: true
hosts:
- cert_expires: Nov 20 22:57:16 2026 GMT
  host: www.becn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 05:18:41 2026 GMT
  host: www.beaconproplus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 05:18:41 2026 GMT
  host: beaconproplus.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Beacon Roofing Supply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beacon Roofing Supply, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Beacon Roofing Supply
provider_slug: beacon-roofing-supply
slug: beacon-roofing-supply-domain-security
source_filename: beacon-roofing-supply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.becn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 22:57:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.beaconproplus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 05:18:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: beaconproplus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 05:18:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: becn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: beaconproplus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beacon-roofing-supply/refs/heads/main/security/beacon-roofing-supply-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Construction
- Distribution
- Roofing
- Building Materials
- E-Commerce
- Fortune 1000
- Supply Chain
- Order
- Catalog
- Delivery
---
