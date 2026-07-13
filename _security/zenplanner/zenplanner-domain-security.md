---
api_specs:
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner People API
  slug: zenplanner-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Memberships API
  slug: zenplanner-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Classes API
  slug: zenplanner-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Locations API
  slug: zenplanner-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Programs API
  slug: zenplanner-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Prospects API
  slug: zenplanner-prospects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
- filename: zenplanner-openapi.yml
  format: yaml
  label: Zen Planner Groups API
  slug: zenplanner-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/openapi/zenplanner-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zenplanner.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: daxko.com
  spf: true
hosts:
- cert_expires: Aug 22 15:26:41 2026 GMT
  host: zenplanner.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: docs.partners.daxko.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.partners.daxko.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zenplanner Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zen Planner, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zen Planner
provider_slug: zenplanner
slug: zenplanner-domain-security
source_filename: zenplanner-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenplanner.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 15:26:41 2026 GMT\n  hsts: false\n- host: docs.partners.daxko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\n- host: api.partners.daxko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zenplanner.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: daxko.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zenplanner/refs/heads/main/security/zenplanner-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fitness
- Gym Management
- Studio Management
- Martial Arts
- Membership
- Scheduling
- Class Booking
- Daxko
---
