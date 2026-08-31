---
api_specs:
- filename: cloud-foundry-apps-api-openapi.yml
  format: yaml
  label: Cloud Foundry Apps API
  slug: cloud-foundry-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-apps-api-openapi.yml
- filename: cloud-foundry-builds-api-openapi.yml
  format: yaml
  label: Cloud Foundry Builds API
  slug: cloud-foundry-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-builds-api-openapi.yml
- filename: cloud-foundry-cloud-foundry-cloud-controller-api-v3-api-openapi.yml
  format: yaml
  label: Cloud Foundry Cloud Foundry Cloud Controller API V3 API
  slug: cloud-foundry-cloud-foundry-cloud-controller-api-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-cloud-foundry-cloud-controller-api-v3-api-openapi.yml
- filename: cloud-foundry-deployments-api-openapi.yml
  format: yaml
  label: Cloud Foundry Deployments API
  slug: cloud-foundry-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-deployments-api-openapi.yml
- filename: cloud-foundry-jobs-api-openapi.yml
  format: yaml
  label: Cloud Foundry Jobs API
  slug: cloud-foundry-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-jobs-api-openapi.yml
- filename: cloud-foundry-organizations-api-openapi.yml
  format: yaml
  label: Cloud Foundry Organizations API
  slug: cloud-foundry-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-organizations-api-openapi.yml
- filename: cloud-foundry-service-instances-api-openapi.yml
  format: yaml
  label: Cloud Foundry Service Instances API
  slug: cloud-foundry-service-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-service-instances-api-openapi.yml
- filename: cloud-foundry-spaces-api-openapi.yml
  format: yaml
  label: Cloud Foundry Spaces API
  slug: cloud-foundry-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloud-foundry/refs/heads/main/openapi/cloud-foundry-spaces-api-openapi.yml
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
- Open-Source
- PaaS
- Platform
---
