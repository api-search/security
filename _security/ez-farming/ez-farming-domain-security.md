---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ez-farming.com
  spf: true
hosts:
- cert_expires: Sep 24 20:43:15 2026 GMT
  host: ez-farming.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ez Farming Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EZ Farming, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: EZ Farming
provider_slug: ez-farming
slug: ez-farming-domain-security
source_filename: ez-farming-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ez-farming.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 20:43:15 2026 GMT\n  hsts: false\ndomains:\n- domain: ez-farming.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ez-farming/refs/heads/main/security/ez-farming-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Agriculture
- Farming
- Investment
- Agtech
- Cooperative
- Land
---
