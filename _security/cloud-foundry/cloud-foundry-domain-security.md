---
api_specs:
- filename: cloud-foundry-cloud-controller-api-v3-openapi.yml
  format: yaml
  label: Cloud Foundry Cloud Controller API v3
  slug: cloud-controller-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-cloud-controller-api-v3-openapi.yml
- filename: cloud-foundry-loggregator-asyncapi.yml
  format: yaml
  label: Cloud Foundry Loggregator
  slug: loggregator
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/asyncapi/cloud-foundry-loggregator-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cloudfoundry.org
  spf: true
hosts:
- cert_expires: Sep 25 22:15:44 2026 GMT
  host: www.cloudfoundry.org
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 22:15:44 2026 GMT
  host: v3-apidocs.cloudfoundry.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 22:15:44 2026 GMT
  host: docs.cloudfoundry.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloud Foundry Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloud Foundry, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Cloud Foundry
provider_slug: cloud-foundry
slug: cloud-foundry-domain-security
source_filename: cloud-foundry-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudfoundry.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:15:44 2026 GMT\n  hsts: true\n  hsts_max_age: 10886400\n- host: v3-apidocs.cloudfoundry.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:15:44 2026 GMT\n  hsts: false\n- host: docs.cloudfoundry.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 22:15:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudfoundry.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/security/cloud-foundry-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Foundry Foundation
- Containers
- Multi-Cloud
- Open Source
- PaaS
- Platform
---
