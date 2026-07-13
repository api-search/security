---
api_specs:
- filename: salesforce-marketing-cloud-openapi.yml
  format: yaml
  label: Marketing Cloud REST API
  slug: marketing-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/openapi/salesforce-marketing-cloud-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: salesforce.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:caa-violations@salesforce.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: marketingcloudapis.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: developer.salesforce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: your_subdomain.rest.marketingcloudapis.com
  https: false
- host: your_subdomain.soap.marketingcloudapis.com
  https: false
kind: domain-security
layout: security
method: probed
name: Salesforce Marketing Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesforce Marketing Cloud, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salesforce Marketing Cloud
provider_slug: salesforce-marketing-cloud
slug: salesforce-marketing-cloud-domain-security
source_filename: salesforce-marketing-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: your_subdomain.rest.marketingcloudapis.com\n  https: false\n- host: your_subdomain.soap.marketingcloudapis.com\n  https: false\ndomains:\n- domain: salesforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: marketingcloudapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:caa-violations@salesforce.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/salesforce-marketing-cloud/refs/heads/main/security/salesforce-marketing-cloud-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Automation
- Customer Journey
- Digital Marketing
- Email
- Marketing
- Personalization
---
