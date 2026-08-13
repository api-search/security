---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ecorobotix.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: ecorobotix.cloud
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: ecorobotix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 15 23:59:59 2027 GMT
  host: portal.ecorobotix.cloud
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ecorobotix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ecorobotix, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ecorobotix
provider_slug: ecorobotix
slug: ecorobotix-domain-security
source_filename: ecorobotix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ecorobotix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\n- host: portal.ecorobotix.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: ecorobotix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ecorobotix.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ecorobotix/refs/heads/main/security/ecorobotix-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Agriculture
- AgTech
- Precision Agriculture
- Robotics
- Artificial Intelligence
- Computer Vision
- Machine Learning
- Sustainability
- Farm Equipment
- Switzerland
- IoT
---
