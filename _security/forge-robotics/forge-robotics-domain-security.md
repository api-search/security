---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: forge-robotics.com
  spf: true
hosts:
- cert_expires: Aug 19 22:52:09 2026 GMT
  host: forge-robotics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forge Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forge Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Forge Robotics
provider_slug: forge-robotics
slug: forge-robotics-domain-security
source_filename: forge-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forge-robotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 22:52:09 2026 GMT\n  hsts: false\ndomains:\n- domain: forge-robotics.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forge-robotics/refs/heads/main/security/forge-robotics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Robotics
- Manufacturing
- Automation
- Autonomous Factories
- Metal Fabrication
- Welding
- Computer Vision
- Y Combinator
---
