---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  - 0 issue "microsoft.com"
  - 0 iodef "mailto:platform-security@getcruise.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@getcruise.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: getcruise.com
  spf: true
hosts:
- cert_expires: Aug 25 23:59:59 2026 GMT
  host: getcruise.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cruise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cruise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cruise
provider_slug: cruise
slug: cruise-domain-security
source_filename: cruise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getcruise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: getcruise.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"microsoft.com\"\n  - 0 iodef \"mailto:platform-security@getcruise.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@getcruise.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cruise/refs/heads/main/security/cruise-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Frontier Tech
- Autonomous Vehicles
- Robotaxi
- Self-Driving
- Automotive
- Mobility
- General Motors
---
