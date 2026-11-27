---
api_specs:
- filename: amazon-msk-clusters-api-openapi.yml
  format: yaml
  label: Amazon MSK Clusters API
  slug: amazon-msk-clusters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-clusters-api-openapi.yml
- filename: amazon-msk-compatible-kafka-versions-api-openapi.yml
  format: yaml
  label: Amazon MSK Compatible Kafka Versions API
  slug: amazon-msk-compatible-kafka-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-compatible-kafka-versions-api-openapi.yml
- filename: amazon-msk-configurations-api-openapi.yml
  format: yaml
  label: Amazon MSK Configurations API
  slug: amazon-msk-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-configurations-api-openapi.yml
- filename: amazon-msk-kafka-versions-api-openapi.yml
  format: yaml
  label: Amazon MSK Kafka Versions API
  slug: amazon-msk-kafka-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-kafka-versions-api-openapi.yml
- filename: amazon-msk-operations-api-openapi.yml
  format: yaml
  label: Amazon MSK Operations API
  slug: amazon-msk-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-operations-api-openapi.yml
- filename: amazon-msk-tags-api-openapi.yml
  format: yaml
  label: Amazon MSK Tags API
  slug: amazon-msk-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-tags-api-openapi.yml
- filename: amazon-msk-channels-api-openapi.yml
  format: yaml
  label: Amazon MSK Msk Channels API
  slug: amazon-msk-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-channels-api-openapi.yml
- filename: amazon-msk-policy-api-openapi.yml
  format: yaml
  label: Amazon MSK Msk Policy API
  slug: amazon-msk-policy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-policy-api-openapi.yml
- filename: amazon-msk-replication-api-openapi.yml
  format: yaml
  label: Amazon MSK Msk Replication API
  slug: amazon-msk-replication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-replication-api-openapi.yml
- filename: amazon-msk-topics-api-openapi.yml
  format: yaml
  label: Amazon MSK Msk Topics API
  slug: amazon-msk-topics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-topics-api-openapi.yml
- filename: amazon-msk-vpc-connection-api-openapi.yml
  format: yaml
  label: Amazon MSK Msk Vpc Connection API
  slug: amazon-msk-vpc-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-vpc-connection-api-openapi.yml
- filename: amazon-msk-connectors-api-openapi.yml
  format: yaml
  label: Amazon MSK Msk Connectors API
  slug: amazon-msk-connectors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-connectors-api-openapi.yml
- filename: amazon-msk-custom-plugins-api-openapi.yml
  format: yaml
  label: Amazon MSK Msk Custom Plugins API
  slug: amazon-msk-custom-plugins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-custom-plugins-api-openapi.yml
- filename: amazon-msk-worker-configurations-api-openapi.yml
  format: yaml
  label: Amazon MSK Msk Worker Configurations API
  slug: amazon-msk-worker-configurations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-msk/openapi/amazon-msk-worker-configurations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amazon.com
  spf: true
hosts:
- cert_expires: Mar  4 23:59:59 2027 GMT
  host: aws.amazon.com
  hsts: true
  hsts_max_age: 47304000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amazon MSK Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amazon MSK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amazon MSK
provider_slug: amazon-msk
slug: amazon-msk-domain-security
source_filename: amazon-msk-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aws.amazon.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 47304000\ndomains:\n- domain: amazon.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amazon-msk/security/amazon-msk-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Amazon Web Services
- Streaming
- Kafka
- Apache Kafka
- Event Streaming
- Data Pipeline
---
