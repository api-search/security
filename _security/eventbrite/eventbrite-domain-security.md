---
api_specs:
- filename: eventbrite-attendees-api-openapi.yml
  format: yaml
  label: Eventbrite Attendees API
  slug: eventbrite-attendees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-attendees-api-openapi.yml
- filename: eventbrite-categories-api-openapi.yml
  format: yaml
  label: Eventbrite Categories API
  slug: eventbrite-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-categories-api-openapi.yml
- filename: eventbrite-events-api-openapi.yml
  format: yaml
  label: Eventbrite Events API
  slug: eventbrite-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-events-api-openapi.yml
- filename: eventbrite-orders-api-openapi.yml
  format: yaml
  label: Eventbrite Orders API
  slug: eventbrite-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-orders-api-openapi.yml
- filename: eventbrite-organizations-api-openapi.yml
  format: yaml
  label: Eventbrite Organizations API
  slug: eventbrite-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-organizations-api-openapi.yml
- filename: eventbrite-ticket-classes-api-openapi.yml
  format: yaml
  label: Eventbrite Ticket Classes API
  slug: eventbrite-ticket-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-ticket-classes-api-openapi.yml
- filename: eventbrite-users-api-openapi.yml
  format: yaml
  label: Eventbrite Users API
  slug: eventbrite-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-users-api-openapi.yml
- filename: eventbrite-venues-api-openapi.yml
  format: yaml
  label: Eventbrite Venues API
  slug: eventbrite-venues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/openapi/eventbrite-venues-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:domains@eventbrite.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eventbrite.com
  spf: true
- caa:
  - 0 issue "awstrust.com"
  - 0 iodef "mailto:domains@eventbrite.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: false
  dnssec: false
  domain: eventbriteapi.com
  spf: false
hosts:
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.eventbrite.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: www.eventbriteapi.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eventbrite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eventbrite, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Eventbrite
provider_slug: eventbrite
slug: eventbrite-domain-security
source_filename: eventbrite-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eventbrite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.eventbriteapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eventbrite.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:domains@eventbrite.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: eventbriteapi.com\n  dnssec: false\n  caa:\n  - 0 issue \"awstrust.com\"\n  - 0 iodef \"mailto:domains@eventbrite.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eventbrite/refs/heads/main/security/eventbrite-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Event
- Event Technology
- Ticketing
- Marketplace
---
