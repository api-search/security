---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: stackav.com
  spf: true
hosts:
- cert_expires: Oct 31 00:07:01 2026 GMT
  host: stackav.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stack Av Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stack AV, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Stack AV
provider_slug: stack-av
slug: stack-av-domain-security
source_filename: stack-av-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stackav.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 00:07:01 2026 GMT\n  hsts: false\ndomains:\n- domain: stackav.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-av/refs/heads/main/security/stack-av-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Autonomous Vehicles
- Transportation
- Trucking
- Freight
- Logistics
- Artificial Intelligence
- Robotics
- Machine Learning
- Open Source
---
