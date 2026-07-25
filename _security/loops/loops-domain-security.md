---
api_specs:
- filename: loops-api-key-api-openapi.yml
  format: yaml
  label: Loops API key API
  slug: loops-api-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-api-key-api-openapi.yml
- filename: loops-campaigns-api-openapi.yml
  format: yaml
  label: Loops Campaigns API
  slug: loops-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-campaigns-api-openapi.yml
- filename: loops-components-api-openapi.yml
  format: yaml
  label: Loops Components API
  slug: loops-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-components-api-openapi.yml
- filename: loops-contact-properties-api-openapi.yml
  format: yaml
  label: Loops Contact properties API
  slug: loops-contact-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-contact-properties-api-openapi.yml
- filename: loops-contacts-api-openapi.yml
  format: yaml
  label: Loops Contacts API
  slug: loops-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-contacts-api-openapi.yml
- filename: loops-dedicated-sending-ips-api-openapi.yml
  format: yaml
  label: Loops Dedicated sending IPs API
  slug: loops-dedicated-sending-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-dedicated-sending-ips-api-openapi.yml
- filename: loops-email-messages-api-openapi.yml
  format: yaml
  label: Loops Email messages API
  slug: loops-email-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-email-messages-api-openapi.yml
- filename: loops-events-api-openapi.yml
  format: yaml
  label: Loops Events API
  slug: loops-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-events-api-openapi.yml
- filename: loops-mailing-lists-api-openapi.yml
  format: yaml
  label: Loops Mailing lists API
  slug: loops-mailing-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-mailing-lists-api-openapi.yml
- filename: loops-themes-api-openapi.yml
  format: yaml
  label: Loops Themes API
  slug: loops-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-themes-api-openapi.yml
- filename: loops-transactional-emails-api-openapi.yml
  format: yaml
  label: Loops Transactional emails API
  slug: loops-transactional-emails-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/openapi/loops-transactional-emails-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: loops.so
  spf: true
hosts:
- cert_expires: Sep 14 20:39:28 2026 GMT
  host: loops.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 18:48:26 2026 GMT
  host: app.loops.so
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loops Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loops, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Loops
provider_slug: loops
slug: loops-domain-security
source_filename: loops-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loops.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:39:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.loops.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:48:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: loops.so\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loops/refs/heads/main/security/loops-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Marketing Automation
- Transactional Email
- SaaS
- Communications
---
