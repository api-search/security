---
api_specs:
- filename: alianza-openapi-original.yml
  format: yaml
  label: Alianza Public API
  slug: alianza-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alianza/refs/heads/main/openapi/alianza-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: alianza.com
  spf: true
hosts:
- cert_expires: Sep 15 09:23:51 2026 GMT
  host: www.alianza.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: developer.alianza.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: api.alianza.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Alianza Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alianza, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Alianza
provider_slug: alianza
slug: alianza-domain-security
source_filename: alianza-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.alianza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 09:23:51 2026 GMT\n  hsts: false\n- host: developer.alianza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.alianza.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: alianza.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alianza/refs/heads/main/security/alianza-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Communications
- Cloud Communications
- Voice
- VoIP
- Telecommunications
- UCaaS
- SIP Trunking
- Telephone Numbers
- CPaaS
- Service Providers
---
