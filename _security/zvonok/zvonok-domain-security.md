---
api_specs:
- filename: zvonok-default-api-openapi.yml
  format: yaml
  label: Zvonok Абонентские номера API
  slug: zvonok-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvonok/openapi/zvonok-default-api-openapi.yml
- filename: zvonok-sip-api-openapi.yml
  format: yaml
  label: Zvonok SIP Линии API
  slug: zvonok-sip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvonok/openapi/zvonok-sip-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zvonok.com
  spf: true
hosts:
- cert_expires: Dec 22 03:53:13 2026 GMT
  host: zvonok.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zvonok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zvonok, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Zvonok
provider_slug: zvonok
slug: zvonok-domain-security
source_filename: zvonok-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zvonok.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 03:53:13 2026 GMT\n  hsts: false\ndomains:\n- domain: zvonok.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/zvonok/security/zvonok-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Telephony
- Automation
- Artificial Intelligence
- Marketing
- Sales
---
