---
api_specs:
- filename: eventship-com-attendees-api-openapi.yml
  format: yaml
  label: Eventship Attendees API
  slug: eventship-com-attendees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventship-com/openapi/eventship-com-attendees-api-openapi.yml
- filename: eventship-com-broadcast-api-openapi.yml
  format: yaml
  label: Eventship Broadcast API
  slug: eventship-com-broadcast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventship-com/openapi/eventship-com-broadcast-api-openapi.yml
- filename: eventship-com-events-api-openapi.yml
  format: yaml
  label: Eventship Events API
  slug: eventship-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventship-com/openapi/eventship-com-events-api-openapi.yml
- filename: eventship-com-hubs-api-openapi.yml
  format: yaml
  label: Eventship Hubs API
  slug: eventship-com-hubs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventship-com/openapi/eventship-com-hubs-api-openapi.yml
- filename: eventship-com-questions-api-openapi.yml
  format: yaml
  label: Eventship Questions API
  slug: eventship-com-questions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventship-com/openapi/eventship-com-questions-api-openapi.yml
- filename: eventship-com-registration-api-openapi.yml
  format: yaml
  label: Eventship Registration API
  slug: eventship-com-registration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventship-com/openapi/eventship-com-registration-api-openapi.yml
- filename: eventship-com-speakers-api-openapi.yml
  format: yaml
  label: Eventship Speakers API
  slug: eventship-com-speakers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventship-com/openapi/eventship-com-speakers-api-openapi.yml
- filename: eventship-com-ticket-types-api-openapi.yml
  format: yaml
  label: Eventship Ticket Types API
  slug: eventship-com-ticket-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventship-com/openapi/eventship-com-ticket-types-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: eventship.com
  spf: true
hosts:
- cert_expires: Dec 31 09:36:40 2026 GMT
  host: eventship.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eventship Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eventship, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Eventship
provider_slug: eventship-com
slug: eventship-com-domain-security
source_filename: eventship-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eventship.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 09:36:40 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: eventship.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eventship-com/security/eventship-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Event
- Attendees
- Ticketing
- Event Management
---
