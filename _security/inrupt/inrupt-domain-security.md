---
api_specs:
- filename: inrupt-discovery-api-openapi.yml
  format: yaml
  label: Inrupt Discovery API
  slug: inrupt-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrupt/refs/heads/main/openapi/inrupt-discovery-api-openapi.yml
- filename: inrupt-jsonkeys-api-openapi.yml
  format: yaml
  label: Inrupt Jsonkeys API
  slug: inrupt-jsonkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrupt/refs/heads/main/openapi/inrupt-jsonkeys-api-openapi.yml
- filename: inrupt-subscription-api-openapi.yml
  format: yaml
  label: Inrupt Subscription API
  slug: inrupt-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrupt/refs/heads/main/openapi/inrupt-subscription-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazontrust.com"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: inrupt.com
  spf: true
hosts:
- cert_expires: Oct 14 11:45:26 2026 GMT
  host: www.inrupt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 06:15:15 2026 GMT
  host: docs.inrupt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  3 03:09:40 2026 GMT
  host: notification.inrupt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inrupt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inrupt, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Inrupt
provider_slug: inrupt
slug: inrupt-domain-security
source_filename: inrupt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.inrupt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 11:45:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.inrupt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 06:15:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: notification.inrupt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  3 03:09:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inrupt.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inrupt/refs/heads/main/security/inrupt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Solid
- Personal Data Stores
- Decentralized Identity
- Data Privacy
- Access Control
- Verifiable Credentials
- Linked Data
- RDF
- Consent Management
- Data Wallets
- Agent Infrastructure
- Model Context Protocol
- Enterprise Software
---
