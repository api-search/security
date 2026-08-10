---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bluewhite.ai
  spf: true
hosts:
- cert_expires: Oct  1 22:45:02 2026 GMT
  host: www.bluewhite.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: compass.bluewhite.ai
  hsts: false
  https: true
  note: Compass operator platform; AWS ALB 302s every path to the Keycloak realm at auth.bluewhite.ai.
  tls_version: TLSv1.2
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: auth.bluewhite.ai
  hsts: false
  https: true
  note: Keycloak identity provider (realm maia-cloud); returned HTTP 503 to anonymous requests on every path probed, including /realms/maia-cloud/.well-known/openid-configuration.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Blue White Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blue White Robotics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Blue White Robotics
provider_slug: blue-white-robotics
slug: blue-white-robotics-domain-security
source_filename: blue-white-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bluewhite.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 22:45:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: compass.bluewhite.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\n  note: Compass operator platform; AWS ALB 302s every path to the Keycloak realm at\n    auth.bluewhite.ai.\n- host: auth.bluewhite.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: false\n  note: Keycloak identity provider (realm maia-cloud); returned HTTP 503 to anonymous\n    requests on every path probed, including /realms/maia-cloud/.well-known/openid-configuration.\ndomains:\n- domain: bluewhite.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-white-robotics/refs/heads/main/security/blue-white-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Autonomous Vehicles
- Agriculture
- Agricultural Technology
- Artificial Intelligence
- Fleet Management
- Defense
- Unmanned Ground Vehicles
- Israel
---
