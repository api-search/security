---
api_specs:
- filename: withlocals-availability-api-openapi.yml
  format: yaml
  label: Withlocals Availability API
  slug: withlocals-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-availability-api-openapi.yml
- filename: withlocals-bookings-api-openapi.yml
  format: yaml
  label: Withlocals Bookings API
  slug: withlocals-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-bookings-api-openapi.yml
- filename: withlocals-products-api-openapi.yml
  format: yaml
  label: Withlocals Products API
  slug: withlocals-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-products-api-openapi.yml
- filename: withlocals-supplier-api-openapi.yml
  format: yaml
  label: Withlocals Supplier API
  slug: withlocals-supplier-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-supplier-api-openapi.yml
- filename: withlocals-webhooks-api-openapi.yml
  format: yaml
  label: Withlocals Webhooks API
  slug: withlocals-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/openapi/withlocals-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: withlocals.com
  spf: true
hosts:
- cert_expires: Dec 11 21:56:40 2026 GMT
  host: www.withlocals.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Withlocals Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Withlocals, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Withlocals
provider_slug: withlocals
slug: withlocals-domain-security
source_filename: withlocals-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.withlocals.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 21:56:40 2026 GMT\n  hsts: false\ndomains:\n- domain: withlocals.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/withlocals/refs/heads/main/security/withlocals-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Travel
- Tours
- Experiences
- Tourism
- Marketplace
- Partner API
---
