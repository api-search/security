---
description: ''
domains:
- caa:
  - 0 issue "godaddy.com"
  - 0 iodef "mailto:devops@modrobotics.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: modrobotics.com
  spf: true
hosts:
- cert_expires: Jan 19 14:16:44 2027 GMT
  host: modrobotics.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Modular Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modular Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Modular Robotics
provider_slug: modular-robotics
slug: modular-robotics-domain-security
source_filename: modular-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: modrobotics.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 19 14:16:44 2027 GMT\n  hsts: false\ndomains:\n- domain: modrobotics.com\n  dnssec: false\n  caa:\n  - 0 issue \"godaddy.com\"\n  - 0 iodef \"mailto:devops@modrobotics.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modular-robotics/refs/heads/main/security/modular-robotics-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Hardware
- Robotics
- Education
- STEM
- EdTech
- Consumer Electronics
---
