---
api_specs:
- filename: openapi
  format: yaml
  label: Root Platform API
  slug: root-platform-api
  spec_type: OpenAPI
  url: https://api.rootplatform.com/v1/docs/insurance/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: joinroot.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: rootplatform.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.joinroot.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:10:36 2026 GMT
  host: docs.rootplatform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 13 23:59:59 2026 GMT
  host: api.rootplatform.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Root Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Root Insurance, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Root Insurance
provider_slug: root
slug: root-domain-security
source_filename: root-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.joinroot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.rootplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:10:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.rootplatform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: joinroot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rootplatform.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/security/root-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Insurance
- Auto Insurance
- Telematics
- Embedded Insurance
- Policy Administration
- Claims
- Usage-Based Insurance
- InsurTech
---
