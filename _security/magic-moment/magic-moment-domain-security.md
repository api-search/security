---
api_specs:
- filename: magic-moment-salesforce-integration-openapi.yml
  format: yaml
  label: Magic Moment Playbook Salesforce Integration API
  slug: magic-moment-playbook-salesforce-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/openapi/magic-moment-salesforce-integration-openapi.yml
- filename: magic-moment-hubspot-integration-openapi.yml
  format: yaml
  label: Magic Moment Playbook HubSpot Integration API
  slug: magic-moment-playbook-hubspot-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/openapi/magic-moment-hubspot-integration-openapi.yml
- filename: magic-moment-office-suite-integration-openapi.yml
  format: yaml
  label: Magic Moment Playbook Office Suite Integration API
  slug: magic-moment-playbook-office-suite-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/openapi/magic-moment-office-suite-integration-openapi.yml
- filename: magic-moment-call-integration-openapi.yml
  format: yaml
  label: Magic Moment Playbook Call Integration API
  slug: magic-moment-playbook-call-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/openapi/magic-moment-call-integration-openapi.yml
- filename: magic-moment-reporting-openapi.yml
  format: yaml
  label: Magic Moment Playbook Reporting API
  slug: magic-moment-playbook-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/openapi/magic-moment-reporting-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magicmoment.jp
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magicmoment.co.jp
  spf: false
hosts:
- cert_expires: Sep 24 10:20:01 2026 GMT
  host: www.magicmoment.jp
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 12:31:36 2026 GMT
  host: magicmoment.jp
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 21:53:41 2026 GMT
  host: sfdc.magicmoment.co.jp
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Magic Moment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magic Moment, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Magic Moment
provider_slug: magic-moment
slug: magic-moment-domain-security
source_filename: magic-moment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.magicmoment.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:20:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: magicmoment.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:31:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: sfdc.magicmoment.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:53:41 2026 GMT\n  hsts: null\ndomains:\n- domain: magicmoment.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: magicmoment.co.jp\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magic-moment/refs/heads/main/security/magic-moment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Enterprise
- Sales
- Artificial Intelligence
- CRM
- Sales Automation
- Software-as-a-Service
- Japan
- Salesforce
- HubSpot
- Sales Enablement
---
