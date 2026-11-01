---
api_specs:
- filename: openapi.json
  format: json
  label: BlackLabel Public Evidence API
  slug: blacklabel-public-evidence-api
  spec_type: OpenAPI
  url: https://blacklabeltec.com/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: blacklabeltec.com
  spf: true
hosts:
- cert_expires: Dec  6 09:07:44 2026 GMT
  host: blacklabeltec.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blacklabeltec Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for blacklabeltec-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: blacklabeltec-com
provider_slug: blacklabeltec-com
slug: blacklabeltec-com-domain-security
source_filename: blacklabeltec-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blacklabeltec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 09:07:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blacklabeltec.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/blacklabeltec-com/security/blacklabeltec-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Software
- AI
- Automation
- Cybersecurity
- CustomSoftware
---
