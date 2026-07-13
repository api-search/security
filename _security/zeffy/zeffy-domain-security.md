---
api_specs:
- filename: zeffy-openapi.yml
  format: yaml
  label: Zeffy Payments API
  slug: zeffy-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeffy/refs/heads/main/openapi/zeffy-openapi.yml
- filename: zeffy-openapi.yml
  format: yaml
  label: Zeffy Contacts API
  slug: zeffy-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeffy/refs/heads/main/openapi/zeffy-openapi.yml
- filename: zeffy-openapi.yml
  format: yaml
  label: Zeffy Campaigns API
  slug: zeffy-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zeffy/refs/heads/main/openapi/zeffy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zeffy.com
  spf: true
hosts:
- cert_expires: Sep 27 07:50:28 2026 GMT
  host: www.zeffy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 30 17:21:28 2026 GMT
  host: support.zeffy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 07:50:53 2026 GMT
  host: api.zeffy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zeffy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zeffy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Zeffy
provider_slug: zeffy
slug: zeffy-domain-security
source_filename: zeffy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zeffy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 07:50:28 2026 GMT\n  hsts: false\n- host: support.zeffy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 17:21:28 2026 GMT\n  hsts: false\n- host: api.zeffy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 07:50:53 2026 GMT\n  hsts: null\ndomains:\n- domain: zeffy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zeffy/refs/heads/main/security/zeffy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Fundraising
- Nonprofit
- Donations
- Payments
- Donor Management
- Free
- Webhooks
---
