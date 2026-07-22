---
api_specs:
- filename: sign-in-enterprise-guest-api-openapi-original.yml
  format: yaml
  label: Sign In Solutions VMS API
  slug: sign-in-solutions-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sign-in-enterprise/refs/heads/main/openapi/sign-in-enterprise-guest-api-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: signinsolutions.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: signinenterprise.com
  spf: true
hosts:
- cert_expires: Oct 17 19:44:47 2026 GMT
  host: signinsolutions.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 16:22:45 2026 GMT
  host: developers.signinenterprise.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 14:49:40 2026 GMT
  host: us.tractionguest.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sign In Enterprise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sign In Enterprise, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sign In Enterprise
provider_slug: sign-in-enterprise
slug: sign-in-enterprise-domain-security
source_filename: sign-in-enterprise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: signinsolutions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 19:44:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.signinenterprise.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 16:22:45 2026 GMT\n  hsts: false\n- host: us.tractionguest.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 14:49:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: signinsolutions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: signinenterprise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sign-in-enterprise/refs/heads/main/security/sign-in-enterprise-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Vertical Software
- Visitor Management
- Physical Security
- Workplace Experience
- Identity
- Compliance
- Access Control
---
