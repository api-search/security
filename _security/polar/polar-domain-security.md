---
api_specs:
- filename: polar-cardio-load-api-openapi.yml
  format: yaml
  label: Polar Cardio load API
  slug: polar-cardio-load-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-cardio-load-api-openapi.yml
- filename: polar-continuous-heart-rate-api-openapi.yml
  format: yaml
  label: Polar Continuous Heart Rate API
  slug: polar-continuous-heart-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-continuous-heart-rate-api-openapi.yml
- filename: polar-daily-activity-api-openapi.yml
  format: yaml
  label: Polar Daily activity API
  slug: polar-daily-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-daily-activity-api-openapi.yml
- filename: polar-daily-activity-deprecated-api-openapi.yml
  format: yaml
  label: Polar Daily activity (deprecated) API
  slug: polar-daily-activity-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-daily-activity-deprecated-api-openapi.yml
- filename: polar-elixir-trade-biosensing-api-openapi.yml
  format: yaml
  label: Polar Elixir&trade; Biosensing API
  slug: polar-elixir-trade-biosensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-elixir-trade-biosensing-api-openapi.yml
- filename: polar-exercises-api-openapi.yml
  format: yaml
  label: Polar Exercises API
  slug: polar-exercises-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-exercises-api-openapi.yml
- filename: polar-exercises-deprecated-api-openapi.yml
  format: yaml
  label: Polar Exercises (deprecated) API
  slug: polar-exercises-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-exercises-deprecated-api-openapi.yml
- filename: polar-nightly-recharge-api-openapi.yml
  format: yaml
  label: Polar Nightly Recharge API
  slug: polar-nightly-recharge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-nightly-recharge-api-openapi.yml
- filename: polar-physical-info-api-openapi.yml
  format: yaml
  label: Polar Physical info API
  slug: polar-physical-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-physical-info-api-openapi.yml
- filename: polar-physical-info-deprecated-api-openapi.yml
  format: yaml
  label: Polar Physical info (deprecated) API
  slug: polar-physical-info-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-physical-info-deprecated-api-openapi.yml
- filename: polar-player-training-sessions-api-openapi.yml
  format: yaml
  label: Polar Player training sessions API
  slug: polar-player-training-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-player-training-sessions-api-openapi.yml
- filename: polar-pull-notifications-api-openapi.yml
  format: yaml
  label: Polar Pull notifications API
  slug: polar-pull-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-pull-notifications-api-openapi.yml
- filename: polar-sleep-api-openapi.yml
  format: yaml
  label: Polar Sleep API
  slug: polar-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-sleep-api-openapi.yml
- filename: polar-sleepwise-trade-api-openapi.yml
  format: yaml
  label: Polar SleepWise&trade; API
  slug: polar-sleepwise-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-sleepwise-trade-api-openapi.yml
- filename: polar-team-api-openapi.yml
  format: yaml
  label: Polar Team API
  slug: polar-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-team-api-openapi.yml
- filename: polar-team-training-sessions-api-openapi.yml
  format: yaml
  label: Polar Team training sessions API
  slug: polar-team-training-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-team-training-sessions-api-openapi.yml
- filename: polar-users-api-openapi.yml
  format: yaml
  label: Polar Users API
  slug: polar-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-users-api-openapi.yml
- filename: polar-webhooks-api-openapi.yml
  format: yaml
  label: Polar Webhooks API
  slug: polar-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/openapi/polar-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: polar.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: polaraccesslink.com
  spf: false
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.polar.com
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 22 23:59:59 2026 GMT
  host: flow.polar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: www.polaraccesslink.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Polar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Polar
provider_slug: polar
slug: polar-domain-security
source_filename: polar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: flow.polar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 22 23:59:59 2026 GMT\n  hsts: false\n- host: www.polaraccesslink.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: polar.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: polaraccesslink.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polar/refs/heads/main/security/polar-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fitness
- Health
- Wearables
- Heart Rate
- Sports
- Training
- Sleep
- Activity Tracking
- Sensors
- Bluetooth
---
