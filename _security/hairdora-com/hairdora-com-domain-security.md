---
api_specs:
- filename: hairdora-com-appointments-api-openapi.yml
  format: yaml
  label: HairDora Appointments API
  slug: hairdora-com-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-appointments-api-openapi.yml
- filename: hairdora-com-clients-api-openapi.yml
  format: yaml
  label: HairDora Clients API
  slug: hairdora-com-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-clients-api-openapi.yml
- filename: hairdora-com-keys-api-openapi.yml
  format: yaml
  label: HairDora Keys API
  slug: hairdora-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-keys-api-openapi.yml
- filename: hairdora-com-salons-api-openapi.yml
  format: yaml
  label: HairDora Salons API
  slug: hairdora-com-salons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-salons-api-openapi.yml
- filename: hairdora-com-services-api-openapi.yml
  format: yaml
  label: HairDora Services API
  slug: hairdora-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-services-api-openapi.yml
- filename: hairdora-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: HairDora Webhook subscriptions API
  slug: hairdora-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hairdora-com/openapi/hairdora-com-webhook-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hairdora.com
  spf: true
hosts:
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: hairdora.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HairDora Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HairDora, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HairDora
provider_slug: hairdora-com
slug: hairdora-com-domain-security
source_filename: hairdora-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hairdora.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: hairdora.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hairdora-com/security/hairdora-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Salon
- Software
- Management
- Booking
- Hair
---
