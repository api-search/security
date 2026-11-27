---
api_specs:
- filename: machineinbox-com-inboxes-api-openapi.yml
  format: yaml
  label: Machine Inbox Inboxes API
  slug: machineinbox-com-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machineinbox-com/openapi/machineinbox-com-inboxes-api-openapi.yml
- filename: machineinbox-com-messages-api-openapi.yml
  format: yaml
  label: Machine Inbox Messages API
  slug: machineinbox-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machineinbox-com/openapi/machineinbox-com-messages-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: machineinbox.com
  spf: true
hosts:
- cert_expires: Jan 12 23:52:26 2027 GMT
  host: machineinbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Machine Inbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Machine Inbox, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Machine Inbox
provider_slug: machineinbox-com
slug: machineinbox-com-domain-security
source_filename: machineinbox-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: machineinbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:52:26 2027 GMT\n  hsts: false\ndomains:\n- domain: machineinbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/machineinbox-com/security/machineinbox-com-domain-security.yml
summary_line: TLSv1.3
tags:
- Email
- Artificial Intelligence
- Automation
- Payments
- Services
- Company
---
