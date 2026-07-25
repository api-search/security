---
api_specs:
- filename: polymath-canbus-api-openapi.yml
  format: yaml
  label: Polymath Robotics CANBus API
  slug: polymath-canbus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-canbus-api-openapi.yml
- filename: polymath-filesystem-api-openapi.yml
  format: yaml
  label: Polymath Robotics filesystem API
  slug: polymath-filesystem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-filesystem-api-openapi.yml
- filename: polymath-health-check-api-openapi.yml
  format: yaml
  label: Polymath Robotics Health Check API
  slug: polymath-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-health-check-api-openapi.yml
- filename: polymath-livekit-api-openapi.yml
  format: yaml
  label: Polymath Robotics Livekit API
  slug: polymath-livekit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-livekit-api-openapi.yml
- filename: polymath-media-api-openapi.yml
  format: yaml
  label: Polymath Robotics Media API
  slug: polymath-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-media-api-openapi.yml
- filename: polymath-ros-api-openapi.yml
  format: yaml
  label: Polymath Robotics ros API
  slug: polymath-ros-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-ros-api-openapi.yml
- filename: polymath-systemd-api-openapi.yml
  format: yaml
  label: Polymath Robotics systemd API
  slug: polymath-systemd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-systemd-api-openapi.yml
- filename: polymath-teleop-control-api-openapi.yml
  format: yaml
  label: Polymath Robotics Teleop Control API
  slug: polymath-teleop-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-teleop-control-api-openapi.yml
- filename: polymath-vehicle-autonomy-api-openapi.yml
  format: yaml
  label: Polymath Robotics Vehicle Autonomy API
  slug: polymath-vehicle-autonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-vehicle-autonomy-api-openapi.yml
- filename: polymath-vehicle-operations-api-openapi.yml
  format: yaml
  label: Polymath Robotics Vehicle Operations API
  slug: polymath-vehicle-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/openapi/polymath-vehicle-operations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: polymathrobotics.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: polymathrobotics.dev
  spf: false
hosts:
- cert_expires: Sep  8 04:45:52 2026 GMT
  host: www.polymathrobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 22:58:57 2026 GMT
  host: synapse.docs.polymathrobotics.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 11:59:59 2026 GMT
  host: polyglot.polymathrobotics.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polymath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polymath Robotics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Polymath Robotics
provider_slug: polymath
slug: polymath-domain-security
source_filename: polymath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.polymathrobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 04:45:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: synapse.docs.polymathrobotics.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 22:58:57 2026 GMT\n  hsts: false\n- host: polyglot.polymathrobotics.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 11:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: polymathrobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: polymathrobotics.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polymath/refs/heads/main/security/polymath-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robotics
- Autonomy
- Industrial Vehicles
- Off-Highway
- Machine Learning
- Simulation
- Teleoperation
- Automation
- Artificial Intelligence
- Unmanned Vehicles
---
