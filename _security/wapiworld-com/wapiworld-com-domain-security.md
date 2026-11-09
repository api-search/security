---
api_specs:
- filename: wapiworld-com-instances-api-openapi.yml
  format: yaml
  label: wapiworld-com Instances API
  slug: wapiworld-com-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-instances-api-openapi.yml
- filename: wapiworld-com-messages-api-openapi.yml
  format: yaml
  label: wapiworld-com Messages API
  slug: wapiworld-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-messages-api-openapi.yml
- filename: wapiworld-com-projects-api-openapi.yml
  format: yaml
  label: wapiworld-com Projects API
  slug: wapiworld-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-projects-api-openapi.yml
- filename: wapiworld-com-webhook-subscriptions-api-openapi.yml
  format: yaml
  label: wapiworld-com Webhook subscriptions API
  slug: wapiworld-com-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wapiworld-com/openapi/wapiworld-com-webhook-subscriptions-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: wapiworld.com
  spf: true
hosts:
- cert_expires: Apr  8 23:59:59 2027 GMT
  host: wapiworld.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wapiworld Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for wapiworld-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: wapiworld-com
provider_slug: wapiworld-com
slug: wapiworld-com-domain-security
source_filename: wapiworld-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wapiworld.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: wapiworld.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/wapiworld-com/security/wapiworld-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Messaging
- WhatsApp
- Developer Platform
- Communications
---
