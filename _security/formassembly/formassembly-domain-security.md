---
api_specs:
- filename: formassembly-formassembly-api-openapi.yml
  format: yaml
  label: FormAssembly REST API
  slug: formassembly-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/openapi/formassembly-formassembly-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: formassembly.com
  spf: true
hosts:
- cert_expires: Sep 15 07:31:05 2026 GMT
  host: www.formassembly.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 15:35:40 2026 GMT
  host: help.formassembly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 23:59:59 2026 GMT
  host: app.formassembly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Formassembly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FormAssembly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: FormAssembly
provider_slug: formassembly
slug: formassembly-domain-security
source_filename: formassembly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.formassembly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 07:31:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.formassembly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 15:35:40 2026 GMT\n  hsts: false\n- host: app.formassembly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: formassembly.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/formassembly/refs/heads/main/security/formassembly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Forms
- Data Collection
- Salesforce
- Enterprise
- HIPAA
- Compliance
- Government
- FedRAMP
- Workflows
- E-Signatures
---
