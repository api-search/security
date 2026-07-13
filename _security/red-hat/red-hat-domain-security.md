---
api_specs:
- filename: openapi
  format: yaml
  label: Red Hat OpenShift API
  slug: red-hat-openshift-api
  spec_type: OpenAPI
  url: https://api.openshift.com/api/clusters_mgmt/v1/openapi
- filename: openapi
  format: yaml
  label: Red Hat OpenShift Cluster Manager API
  slug: red-hat-openshift-cluster-manager-api
  spec_type: OpenAPI
  url: https://api.openshift.com/api/clusters_mgmt/v1/openapi
- filename: red-hat-ansible-automation-platform-openapi.yml
  format: yaml
  label: Red Hat Ansible Automation Platform API
  slug: red-hat-ansible-automation-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/openapi/red-hat-ansible-automation-platform-openapi.yml
- filename: discovery
  format: yaml
  label: Red Hat Quay API
  slug: red-hat-quay-api
  spec_type: OpenAPI
  url: https://quay.io/api/v1/discovery
- filename: red-hat-insights-openapi.yml
  format: yaml
  label: Red Hat Insights API
  slug: red-hat-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/openapi/red-hat-insights-openapi.yml
- filename: red-hat-satellite-openapi.yml
  format: yaml
  label: Red Hat Satellite API
  slug: red-hat-satellite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/openapi/red-hat-satellite-openapi.yml
- filename: red-hat-keycloak-admin-openapi.yml
  format: yaml
  label: Red Hat Build of Keycloak Admin REST API
  slug: red-hat-build-of-keycloak-admin-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/openapi/red-hat-keycloak-admin-openapi.yml
- filename: red-hat-kafka-bridge-asyncapi.yml
  format: yaml
  label: Red Hat Streams for Apache Kafka Bridge API
  slug: red-hat-streams-for-apache-kafka-bridge-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/asyncapi/red-hat-kafka-bridge-asyncapi.yml
- filename: red-hat-notifications-webhooks-asyncapi.yml
  format: yaml
  label: Red Hat Notifications API
  slug: red-hat-notifications-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/asyncapi/red-hat-notifications-webhooks-asyncapi.yml
- filename: openapi
  format: yaml
  label: Red Hat Assisted Installer API
  slug: red-hat-assisted-installer-api
  spec_type: OpenAPI
  url: https://api.openshift.com/api/assisted-install/v2/openapi
description: ''
domains:
- caa:
  - 0 iodef "mailto:it-cert-admin@redhat.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: redhat.com
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: developers.redhat.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.redhat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: console.redhat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Red Hat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Hat, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Red Hat
provider_slug: red-hat
slug: red-hat-domain-security
source_filename: red-hat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: null\n- host: www.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: console.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: redhat.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:it-cert-admin@redhat.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat/refs/heads/main/security/red-hat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- Linux
- Open Source
---
