---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: xenex.com
  spf: true
hosts:
- cert_expires: Oct  3 00:54:17 2026 GMT
  host: xenex.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xenex Disinfection Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Xenex Disinfection Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Xenex Disinfection Services
provider_slug: xenex-disinfection-services
slug: xenex-disinfection-services-domain-security
source_filename: xenex-disinfection-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xenex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 00:54:17 2026 GMT\n  hsts: false\ndomains:\n- domain: xenex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xenex-disinfection-services/refs/heads/main/security/xenex-disinfection-services-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- UV Disinfection
- Medical Devices
- Healthcare
- Infection Prevention
- Robotics
- Hospital Operations
---
