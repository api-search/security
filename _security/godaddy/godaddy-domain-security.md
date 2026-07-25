---
api_specs:
- filename: godaddy-actions-api-openapi.yml
  format: yaml
  label: GoDaddy Actions API
  slug: godaddy-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-actions-api-openapi.yml
- filename: godaddy-contacts-api-openapi.yml
  format: yaml
  label: GoDaddy Contacts API
  slug: godaddy-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-contacts-api-openapi.yml
- filename: godaddy-domains-api-openapi.yml
  format: yaml
  label: GoDaddy Domains API
  slug: godaddy-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-domains-api-openapi.yml
- filename: godaddy-expiry-auctions-registrar-partners-api-openapi.yml
  format: yaml
  label: 'GoDaddy Expiry Auctions: Registrar Partners API'
  slug: godaddy-expiry-auctions-registrar-partners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-expiry-auctions-registrar-partners-api-openapi.yml
- filename: godaddy-notifications-api-openapi.yml
  format: yaml
  label: GoDaddy Notifications API
  slug: godaddy-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-notifications-api-openapi.yml
- filename: godaddy-v1-api-openapi.yml
  format: yaml
  label: GoDaddy v1 API
  slug: godaddy-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-v1-api-openapi.yml
- filename: godaddy-v2-api-openapi.yml
  format: yaml
  label: GoDaddy v2 API
  slug: godaddy-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/openapi/godaddy-v2-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: godaddy.com
  spf: true
hosts:
- cert_expires: Nov  2 23:48:17 2026 GMT
  host: www.godaddy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:48:17 2026 GMT
  host: developer.godaddy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  2 23:48:17 2026 GMT
  host: api.godaddy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Godaddy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GoDaddy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GoDaddy
provider_slug: godaddy
slug: godaddy-domain-security
source_filename: godaddy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.godaddy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:48:17 2026 GMT\n  hsts: null\n- host: developer.godaddy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:48:17 2026 GMT\n  hsts: false\n- host: api.godaddy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 23:48:17 2026 GMT\n  hsts: null\ndomains:\n- domain: godaddy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/godaddy/refs/heads/main/security/godaddy-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Aftermarket
- Certificates
- DNS
- Domains
- Hosting
- Registrar
---
