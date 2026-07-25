---
api_specs:
- filename: amazon-datazone-assets-api-openapi.yml
  format: yaml
  label: Amazon DataZone Assets API
  slug: amazon-datazone-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-assets-api-openapi.yml
- filename: amazon-datazone-domains-api-openapi.yml
  format: yaml
  label: Amazon DataZone Domains API
  slug: amazon-datazone-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-domains-api-openapi.yml
- filename: amazon-datazone-environments-api-openapi.yml
  format: yaml
  label: Amazon DataZone Environments API
  slug: amazon-datazone-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-environments-api-openapi.yml
- filename: amazon-datazone-listings-api-openapi.yml
  format: yaml
  label: Amazon DataZone Listings API
  slug: amazon-datazone-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-listings-api-openapi.yml
- filename: amazon-datazone-projects-api-openapi.yml
  format: yaml
  label: Amazon DataZone Projects API
  slug: amazon-datazone-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-projects-api-openapi.yml
- filename: amazon-datazone-subscriptions-api-openapi.yml
  format: yaml
  label: Amazon DataZone Subscriptions API
  slug: amazon-datazone-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/openapi/amazon-datazone-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazonaws.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
- host: datazone.amazonaws.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amazon Datazone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon DataZone, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon DataZone
provider_slug: amazon-datazone
slug: amazon-datazone-domain-security
source_filename: amazon-datazone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 47304000\n- host: datazone.amazonaws.com\n  https: false\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amazonaws.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-datazone/refs/heads/main/security/amazon-datazone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Catalog
- Data Governance
- Data Management
- Data Sharing
- Analytics
---
