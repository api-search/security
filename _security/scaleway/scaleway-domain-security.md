---
api_specs:
- filename: scaleway-instance-openapi.yml
  format: yaml
  label: Scaleway Instance API
  slug: scaleway-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-instance-openapi.yml
- filename: scaleway-kubernetes-openapi.yml
  format: yaml
  label: Scaleway Kubernetes API
  slug: scaleway-kubernetes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-kubernetes-openapi.yml
- filename: scaleway-iam-openapi.yml
  format: yaml
  label: Scaleway IAM API
  slug: scaleway-iam-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-iam-openapi.yml
- filename: scaleway-load-balancer-openapi.yml
  format: yaml
  label: Scaleway Load Balancer API
  slug: scaleway-load-balancer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-load-balancer-openapi.yml
- filename: scaleway-database-openapi.yml
  format: yaml
  label: Scaleway Managed Database API
  slug: scaleway-database-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-database-openapi.yml
- filename: scaleway-vpc-openapi.yml
  format: yaml
  label: Scaleway VPC API
  slug: scaleway-vpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-vpc-openapi.yml
- filename: scaleway-serverless-containers-openapi.yml
  format: yaml
  label: Scaleway Serverless Containers API
  slug: scaleway-serverless-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-serverless-containers-openapi.yml
- filename: scaleway-serverless-functions-openapi.yml
  format: yaml
  label: Scaleway Serverless Functions API
  slug: scaleway-serverless-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-serverless-functions-openapi.yml
- filename: scaleway-secret-manager-openapi.yml
  format: yaml
  label: Scaleway Secret Manager API
  slug: scaleway-secret-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-secret-manager-openapi.yml
- filename: scaleway-transactional-email-openapi.yml
  format: yaml
  label: Scaleway Transactional Email API
  slug: scaleway-transactional-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/openapi/scaleway-transactional-email-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "zerossl.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@scaleway.com"
  - 0 issuewild "identrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: scaleway.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: www.scaleway.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: api.scaleway.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scaleway Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scaleway, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Scaleway
provider_slug: scaleway
slug: scaleway-domain-security
source_filename: scaleway-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scaleway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.scaleway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: scaleway.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"zerossl.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@scaleway.com\"\n  - 0 issuewild \"identrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scaleway/refs/heads/main/security/scaleway-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Cloud Computing
- Containers
- Database
- European Cloud
- Infrastructure
- Kubernetes
- Serverless
- Storage
---
