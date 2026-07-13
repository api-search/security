---
api_specs:
- filename: jumpcloud-openapi.yml
  format: yaml
  label: JumpCloud API V1
  slug: v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jumpcloud/refs/heads/main/openapi/jumpcloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jumpcloud.com
  spf: true
hosts:
- cert_expires: Sep 13 08:47:43 2026 GMT
  host: jumpcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 07:03:18 2026 GMT
  host: docs.jumpcloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 08:44:56 2026 GMT
  host: console.jumpcloud.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jumpcloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JumpCloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: JumpCloud
provider_slug: jumpcloud
slug: jumpcloud-domain-security
source_filename: jumpcloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jumpcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 08:47:43 2026 GMT\n  hsts: false\n- host: docs.jumpcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 07:03:18 2026 GMT\n  hsts: false\n- host: console.jumpcloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 08:44:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jumpcloud.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jumpcloud/refs/heads/main/security/jumpcloud-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Identity
- Directory Services
- SSO
- MFA
- Device Management
- MDM
- IT Operations
- Zero Trust
---
