---
api_specs:
- filename: microsoft-azure-traffic-manager-providers-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager Providers API
  slug: microsoft-azure-traffic-manager-providers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-traffic-manager/openapi/microsoft-azure-traffic-manager-providers-api-openapi.yml
- filename: microsoft-azure-traffic-manager-subscriptions-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager Subscriptions API
  slug: microsoft-azure-traffic-manager-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-traffic-manager/openapi/microsoft-azure-traffic-manager-subscriptions-api-openapi.yml
- filename: microsoft-azure-traffic-manager-trafficmanagergeographichierarchies-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager Traffic Manager Geographic Hierarchies API
  slug: microsoft-azure-traffic-manager-trafficmanagergeographichierarchies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-traffic-manager/openapi/microsoft-azure-traffic-manager-trafficmanagergeographichierarchies-api-openapi.yml
- filename: microsoft-azure-traffic-manager-usermetricsmodels-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager User Metrics Models API
  slug: microsoft-azure-traffic-manager-usermetricsmodels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-traffic-manager/openapi/microsoft-azure-traffic-manager-usermetricsmodels-api-openapi.yml
- filename: microsoft-azure-traffic-manager-endpoints-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager Endpoints API
  slug: microsoft-azure-traffic-manager-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-traffic-manager/openapi/microsoft-azure-traffic-manager-endpoints-api-openapi.yml
- filename: microsoft-azure-traffic-manager-geographichierarchies-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager Geographic Hierarchies API
  slug: microsoft-azure-traffic-manager-geographichierarchies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-traffic-manager/openapi/microsoft-azure-traffic-manager-geographichierarchies-api-openapi.yml
- filename: microsoft-azure-traffic-manager-heatmap-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager Heat Map API
  slug: microsoft-azure-traffic-manager-heatmap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-traffic-manager/openapi/microsoft-azure-traffic-manager-heatmap-api-openapi.yml
- filename: microsoft-azure-traffic-manager-usermetrics-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager User Metrics API
  slug: microsoft-azure-traffic-manager-usermetrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-traffic-manager/openapi/microsoft-azure-traffic-manager-usermetrics-api-openapi.yml
- filename: microsoft-azure-traffic-manager-profiles-api-openapi.yml
  format: yaml
  label: Azure Traffic Manager Profiles API
  slug: microsoft-azure-traffic-manager-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-traffic-manager/openapi/microsoft-azure-traffic-manager-profiles-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 19:05:38 2027 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Azure Traffic Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Traffic Manager, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Traffic Manager
provider_slug: microsoft-azure-traffic-manager
slug: microsoft-azure-traffic-manager-domain-security
source_filename: microsoft-azure-traffic-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 19:05:38 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-traffic-manager/security/microsoft-azure-traffic-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- DNS Load Balancing
- Failover
- Global Routing
- Networking
- Traffic Distribution
- Traffic Manager
---
