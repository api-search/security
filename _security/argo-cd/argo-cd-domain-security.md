---
api_specs:
- filename: argo-cd-accountservice-api-openapi.yml
  format: yaml
  label: Argo CD AccountService API
  slug: argo-cd-accountservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-accountservice-api-openapi.yml
- filename: argo-cd-applicationservice-api-openapi.yml
  format: yaml
  label: Argo CD ApplicationService API
  slug: argo-cd-applicationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-applicationservice-api-openapi.yml
- filename: argo-cd-applicationsetservice-api-openapi.yml
  format: yaml
  label: Argo CD ApplicationSetService API
  slug: argo-cd-applicationsetservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-applicationsetservice-api-openapi.yml
- filename: argo-cd-certificateservice-api-openapi.yml
  format: yaml
  label: Argo CD CertificateService API
  slug: argo-cd-certificateservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-certificateservice-api-openapi.yml
- filename: argo-cd-clusterservice-api-openapi.yml
  format: yaml
  label: Argo CD ClusterService API
  slug: argo-cd-clusterservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-clusterservice-api-openapi.yml
- filename: argo-cd-gpgkeyservice-api-openapi.yml
  format: yaml
  label: Argo CD GPGKeyService API
  slug: argo-cd-gpgkeyservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-gpgkeyservice-api-openapi.yml
- filename: argo-cd-notificationservice-api-openapi.yml
  format: yaml
  label: Argo CD NotificationService API
  slug: argo-cd-notificationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-notificationservice-api-openapi.yml
- filename: argo-cd-projectservice-api-openapi.yml
  format: yaml
  label: Argo CD ProjectService API
  slug: argo-cd-projectservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-projectservice-api-openapi.yml
- filename: argo-cd-repocredsservice-api-openapi.yml
  format: yaml
  label: Argo CD RepoCredsService API
  slug: argo-cd-repocredsservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-repocredsservice-api-openapi.yml
- filename: argo-cd-repositoryservice-api-openapi.yml
  format: yaml
  label: Argo CD RepositoryService API
  slug: argo-cd-repositoryservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-repositoryservice-api-openapi.yml
- filename: argo-cd-sessionservice-api-openapi.yml
  format: yaml
  label: Argo CD SessionService API
  slug: argo-cd-sessionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-sessionservice-api-openapi.yml
- filename: argo-cd-settingsservice-api-openapi.yml
  format: yaml
  label: Argo CD SettingsService API
  slug: argo-cd-settingsservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-settingsservice-api-openapi.yml
- filename: argo-cd-versionservice-api-openapi.yml
  format: yaml
  label: Argo CD VersionService API
  slug: argo-cd-versionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/openapi/argo-cd-versionservice-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Aug 27 13:13:23 2026 GMT
  host: argo-cd.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Argo Cd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Argo CD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Argo CD
provider_slug: argo-cd
slug: argo-cd-domain-security
source_filename: argo-cd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: argo-cd.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 13:13:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argo-cd/refs/heads/main/security/argo-cd-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Continuous Delivery
- Containers
- Deployment
- GitOps
- Kubernetes
- CNCF
- Open-Source
---
