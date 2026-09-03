---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vatn.com
  spf: true
hosts:
- cert_expires: Nov 27 14:26:00 2026 GMT
  host: www.vatn.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vatn Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vatn Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vatn Systems
provider_slug: vatn-systems
slug: vatn-systems-domain-security
source_filename: vatn-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vatn.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 14:26:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vatn.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatn-systems/refs/heads/main/security/vatn-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defense
- Autonomous Systems
- Maritime
- Robotics
- Underwater Vehicles
- Navigation
- Sensor Fusion
- Hardware
---
