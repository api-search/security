---
api_specs:
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Clients & CRM API
  slug: pixieset-studio-clients-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Sessions & Booking API
  slug: pixieset-studio-sessions-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Invoices & Payments API
  slug: pixieset-studio-invoices-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Studio Contracts API
  slug: pixieset-studio-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
- filename: pixieset-openapi.yml
  format: yaml
  label: Pixieset Gallery Collections & Delivery API
  slug: pixieset-gallery-collections-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/openapi/pixieset-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pixieset.com
  spf: true
hosts:
- cert_expires: Sep  3 19:49:07 2026 GMT
  host: pixieset.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 19:49:07 2026 GMT
  host: studio.pixieset.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 19:49:07 2026 GMT
  host: galleries.pixieset.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixieset Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixieset, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Pixieset
provider_slug: pixieset
slug: pixieset-domain-security
source_filename: pixieset-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pixieset.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:49:07 2026 GMT\n  hsts: false\n- host: studio.pixieset.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:49:07 2026 GMT\n  hsts: false\n- host: galleries.pixieset.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 19:49:07 2026 GMT\n  hsts: false\ndomains:\n- domain: pixieset.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixieset/refs/heads/main/security/pixieset-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Photography
- Client Galleries
- Studio Management
- CRM
- Booking
- Invoicing
- Contracts
- No Public API
---
