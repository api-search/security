---
api_specs:
- filename: akamai-api-definitions-openapi.json
  format: json
  label: Akamai API Endpoint Definition API
  slug: akamai-api-endpoint-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-api-definitions-openapi.json
- filename: akamai-application-security-openapi.json
  format: json
  label: Akamai Application Security API
  slug: akamai-application-security-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-application-security-openapi.json
- filename: akamai-cps-openapi.json
  format: json
  label: Akamai Certificate Provisioning System API
  slug: akamai-certificate-provisioning-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-cps-openapi.json
- filename: akamai-cp-codes-openapi.json
  format: json
  label: Akamai CP Codes and Reporting Groups API
  slug: akamai-cp-codes-and-reporting-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-cp-codes-openapi.json
- filename: webhooks-asyncapi.yml
  format: yaml
  label: Akamai DataStream 2 API V2
  slug: akamai-datastream-2-api-v2
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/webhooks-asyncapi.yml
- filename: akamai-edgekv-openapi.json
  format: json
  label: Akamai EdgeKV API
  slug: akamai-edgekv-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-edgekv-openapi.json
- filename: akamai-edgeworkers-openapi.json
  format: json
  label: Akamai EdgeWorkers API
  slug: akamai-edgeworkers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-edgeworkers-openapi.json
- filename: akamai-fast-purge-openapi.json
  format: json
  label: Akamai Fast Purge API
  slug: akamai-fast-purge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-fast-purge-openapi.json
- filename: webhooks-asyncapi.yml
  format: yaml
  label: Akamai Identity Cloud Webhooks V3 API
  slug: akamai-identity-cloud-webhooks-v3-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/webhooks-asyncapi.yml
- filename: akamai-network-lists-openapi.json
  format: json
  label: Akamai Network Lists API
  slug: akamai-network-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-network-lists-openapi.json
- filename: akamai-papi-openapi.json
  format: json
  label: Akamai Property Manager API
  slug: akamai-property-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-papi-openapi.json
- filename: akamai-sandbox-openapi.json
  format: json
  label: Akamai Sandbox API
  slug: akamai-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-sandbox-openapi.json
- filename: akamai-siem-openapi.json
  format: json
  label: Akamai SIEM Integration API
  slug: akamai-siem-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-siem-openapi.json
- filename: akamai-site-shield-openapi.json
  format: json
  label: Akamai Site Shield API
  slug: akamai-site-shield-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/openapi/akamai-site-shield-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: akamai.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.akamai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 06:16:17 2026 GMT
  host: techdocs.akamai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akamai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akamai, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Akamai
provider_slug: akamai
slug: akamai-domain-security
source_filename: akamai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akamai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n- host: techdocs.akamai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:16:17 2026 GMT\n  hsts: null\ndomains:\n- domain: akamai.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akamai/refs/heads/main/security/akamai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- CDN
- Cloud
- Edge Computing
- Networks
- Platform
- Security
---
