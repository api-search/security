---
api_specs:
- filename: envoisms-ma-api-openapi.json
  format: json
  label: EnvoiSMS API API
  slug: envoisms-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envoisms-ma/openapi/_original/envoisms-ma-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: envoisms.ma
  spf: true
hosts:
- cert_expires: Dec 12 16:10:41 2026 GMT
  host: envoisms.ma
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Envoisms Ma Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for envoisms-ma, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: envoisms-ma
provider_slug: envoisms-ma
slug: envoisms-ma-domain-security
source_filename: envoisms-ma-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: envoisms.ma\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 16:10:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: envoisms.ma\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/envoisms-ma/security/envoisms-ma-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- SMS
- WhatsApp
- Messaging
- Morocco
- CPaaS
---
