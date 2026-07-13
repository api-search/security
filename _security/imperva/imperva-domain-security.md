---
api_specs:
- filename: cwaf-v1-swagger-3.json
  format: json
  label: Imperva Cloud Application Security API
  slug: cloud-application-security-api
  spec_type: OpenAPI
  url: https://github.com/imperva/imperva-web-api-composer/blob/master/src/assets/cwaf/cwaf-v1-swagger-3.json
- filename: securesphere-swagger
  format: yaml
  label: Imperva SecureSphere Open API
  slug: securesphere-open-api
  spec_type: OpenAPI
  url: https://github.com/imperva-dev/securesphere-swagger
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: imperva.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thalesgroup.com
  spf: true
hosts:
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: www.imperva.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 17:17:26 2026 GMT
  host: docs-cybersec.thalesgroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 02:59:24 2026 GMT
  host: api.imperva.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Imperva Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Imperva, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Imperva
provider_slug: imperva
slug: imperva-domain-security
source_filename: imperva-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.imperva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs-cybersec.thalesgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:17:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.imperva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 02:59:24 2026 GMT\n  hsts: null\ndomains:\n- domain: imperva.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: thalesgroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imperva/refs/heads/main/security/imperva-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Security
- Cybersecurity
- WAF
- DDoS Protection
- API Security
- Bot Management
- Data Security
- Cloud Security
---
