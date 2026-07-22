---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: superiorenergy.com
  spf: true
hosts:
- cert_expires: Oct  5 16:21:39 2026 GMT
  host: superiorenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Superior Energy Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Superior Energy Services, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Superior Energy Services
provider_slug: superior-energy-services
slug: superior-energy-services-domain-security
source_filename: superior-energy-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: superiorenergy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:21:39 2026 GMT\n  hsts: false\ndomains:\n- domain: superiorenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superior-energy-services/refs/heads/main/security/superior-energy-services-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Oil And Gas
- Oilfield Services
- Energy
- Well Services
- Drilling
- Completion Tools
- Well Intervention
- Production Services
- Industrial
---
