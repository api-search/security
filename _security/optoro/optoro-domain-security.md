---
api_specs:
- filename: optoro-auth-openapi.yml
  format: yaml
  label: Optoro Auth API
  slug: optoro-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-auth-openapi.yml
- filename: optoro-catalogs-openapi.yml
  format: yaml
  label: Optoro Catalogs API
  slug: optoro-catalogs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-catalogs-openapi.yml
- filename: optoro-facilities-openapi.yml
  format: yaml
  label: Optoro Facilities API
  slug: optoro-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-facilities-openapi.yml
- filename: optoro-rtv-openapi.yml
  format: yaml
  label: Optoro RTV Vendor API
  slug: optoro-rtv-vendor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-rtv-openapi.yml
- filename: optoro-asn-openapi.yml
  format: yaml
  label: Optoro Inbound ASN API
  slug: optoro-inbound-asn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-asn-openapi.yml
- filename: optoro-external-bin-changes-openapi.yml
  format: yaml
  label: Optoro External Bin Changes API
  slug: optoro-external-bin-changes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-external-bin-changes-openapi.yml
- filename: optoro-drop-ship-openapi.yml
  format: yaml
  label: Optoro Drop Ship API
  slug: optoro-drop-ship-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-drop-ship-openapi.yml
- filename: optoro-returns-portal-orders-openapi.yml
  format: yaml
  label: Optoro Returns Portal Orders API
  slug: optoro-returns-portal-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-returns-portal-orders-openapi.yml
- filename: optoro-rmas-openapi.yml
  format: yaml
  label: Optoro Event Webhooks and Customer Endpoints
  slug: optoro-event-webhooks-and-customer-endpoints
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/openapi/optoro-rmas-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: optoro.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: optiturn.com
  spf: false
hosts:
- cert_expires: Oct 16 19:24:36 2026 GMT
  host: www.optoro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 24 07:20:34 2026 GMT
  host: developer.optoro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 04:17:37 2026 GMT
  host: auth.optiturn.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optoro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optoro, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Optoro
provider_slug: optoro
slug: optoro-domain-security
source_filename: optoro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.optoro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 19:24:36 2026 GMT\n  hsts: false\n- host: developer.optoro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 24 07:20:34 2026 GMT\n  hsts: false\n- host: auth.optiturn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 04:17:37 2026 GMT\n  hsts: false\ndomains:\n- domain: optoro.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: optiturn.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optoro/refs/heads/main/security/optoro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Returns Management
- Reverse Logistics
- Retail
- Supply Chain
- eCommerce
- Fulfillment
- Drop Ship
- Inventory
- Webhooks
- Order Management
---
