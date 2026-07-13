---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: energidataservice.dk
  spf: true
hosts:
- cert_expires: Sep 19 06:21:46 2026 GMT
  host: www.energidataservice.dk
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Danish Data Service Energi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Danish data service Energi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Danish data service Energi
provider_slug: danish-data-service-energi
slug: danish-data-service-energi-domain-security
source_filename: danish-data-service-energi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.energidataservice.dk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 19 06:21:46 2026 GMT\n  hsts: null\ndomains:\n- domain: energidataservice.dk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/danish-data-service-energi/refs/heads/main/security/danish-data-service-energi-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Environment
- Public APIs
---
