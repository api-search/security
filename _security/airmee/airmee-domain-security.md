---
api_specs:
- filename: airmee-integration-api-openapi.yml
  format: yaml
  label: Airmee Integration API
  slug: airmee-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airmee/refs/heads/main/openapi/airmee-integration-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: airmee.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: airmee.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: integration.docs.airmee.com.s3-website-eu-west-1.amazonaws.com
  https: false
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: api.airmee.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Airmee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Airmee, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Airmee
provider_slug: airmee
slug: airmee-domain-security
source_filename: airmee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: airmee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\n- host: integration.docs.airmee.com.s3-website-eu-west-1.amazonaws.com\n  https: false\n- host: api.airmee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: airmee.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airmee/refs/heads/main/security/airmee-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Logistics
- Last Mile Delivery
- Shipping
- Parcel Delivery
- Parcel Lockers
- Returns
- E-Commerce
- Same-Day Delivery
- Sweden
- Carrier
---
