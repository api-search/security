---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kinvey.com
  spf: true
hosts:
- host: kinvey.com
  https: false
kind: domain-security
layout: security
method: probed
name: Kinvey Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kinvey, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kinvey
provider_slug: kinvey
slug: kinvey-domain-security
source_filename: kinvey-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kinvey.com\n  https: false\ndomains:\n- domain: kinvey.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinvey/refs/heads/main/security/kinvey-domain-security.yml
summary_line: DMARC
tags:
- Company
- Backend as a Service
- BaaS
- Mobile
- SDK
- Serverless
- Data Storage
- Authentication
- Push Notifications
---
