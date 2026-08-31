---
api_specs:
- filename: service-cloud-bot-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Bot API
  slug: service-cloud-bot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-bot-api-openapi.yml
- filename: service-cloud-health-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Health API
  slug: service-cloud-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-health-api-openapi.yml
- filename: service-cloud-versions-api-openapi.yml
  format: yaml
  label: Salesforce Service Cloud APIs Versions API
  slug: service-cloud-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/openapi/service-cloud-versions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: salesforce.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sfdc.sh
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: developer.salesforce.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: runtime-api-na-west.prod.chatbots.sfdc.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 28 23:59:59 2027 GMT
  host: runtime-api-na-east.prod.chatbots.sfdc.sh
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Service Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Salesforce Service Cloud APIs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Salesforce Service Cloud APIs
provider_slug: service-cloud
slug: service-cloud-domain-security
source_filename: service-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.salesforce.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: null\n- host: runtime-api-na-west.prod.chatbots.sfdc.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: null\n- host: runtime-api-na-east.prod.chatbots.sfdc.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 28 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: salesforce.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: sfdc.sh\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/service-cloud/refs/heads/main/security/service-cloud-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cloud
- CRM
- Customer-Service
- Enterprise
- Salesforce
- Support
---
