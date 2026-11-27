---
api_specs:
- filename: mareaalcalina-com-me-api-openapi.yml
  format: yaml
  label: Marea Alcalina Me API
  slug: mareaalcalina-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mareaalcalina-com/openapi/mareaalcalina-com-me-api-openapi.yml
- filename: mareaalcalina-com-storefronts-api-openapi.yml
  format: yaml
  label: Marea Alcalina Storefronts API
  slug: mareaalcalina-com-storefronts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mareaalcalina-com/openapi/mareaalcalina-com-storefronts-api-openapi.yml
- filename: mareaalcalina-com-users-api-openapi.yml
  format: yaml
  label: Marea Alcalina Users API
  slug: mareaalcalina-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mareaalcalina-com/openapi/mareaalcalina-com-users-api-openapi.yml
- filename: mareaalcalina-com-webhook-endpoints-api-openapi.yml
  format: yaml
  label: Marea Alcalina Webhook Endpoints API
  slug: mareaalcalina-com-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mareaalcalina-com/openapi/mareaalcalina-com-webhook-endpoints-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mareaalcalina.com
  spf: true
hosts:
- cert_expires: May 31 00:50:06 2027 GMT
  host: mareaalcalina.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Marea Alcalina Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Marea Alcalina, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Marea Alcalina
provider_slug: mareaalcalina-com
slug: mareaalcalina-com-domain-security
source_filename: mareaalcalina-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mareaalcalina.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 31 00:50:06 2027 GMT\n  hsts: false\ndomains:\n- domain: mareaalcalina.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mareaalcalina-com/security/mareaalcalina-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
