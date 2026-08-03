---
api_specs:
- filename: outsystems-user-access-management-api-v1-openapi.json
  format: json
  label: OutSystems ODC User and Access Management API
  slug: user-access-management-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-user-access-management-api-v1-openapi.json
- filename: outsystems-portfolio-api-v2-openapi.json
  format: json
  label: OutSystems ODC Portfolio API
  slug: portfolio-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-portfolio-api-v2-openapi.json
- filename: outsystems-portfolio-api-v1-openapi.json
  format: json
  label: OutSystems ODC Portfolio API (v1)
  slug: portfolio-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-portfolio-api-v1-openapi.json
- filename: outsystems-asset-repository-api-v1-openapi.json
  format: json
  label: OutSystems ODC Asset Repository API
  slug: asset-repository-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-asset-repository-api-v1-openapi.json
- filename: outsystems-asset-configurations-api-v1-openapi.json
  format: json
  label: OutSystems ODC Asset Configurations API
  slug: asset-configurations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-asset-configurations-api-v1-openapi.json
- filename: outsystems-environment-configurations-api-v1-openapi.json
  format: json
  label: OutSystems ODC Environment Configurations API
  slug: environment-configurations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-environment-configurations-api-v1-openapi.json
- filename: outsystems-build-operations-api-v1-openapi.json
  format: json
  label: OutSystems ODC Build Operations API
  slug: build-operations-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-build-operations-api-v1-openapi.json
- filename: outsystems-deployments-api-v1-openapi.json
  format: json
  label: OutSystems ODC Deployments API
  slug: deployments-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-deployments-api-v1-openapi.json
- filename: outsystems-dependency-management-api-v1-openapi.json
  format: json
  label: OutSystems ODC Dependency Management API
  slug: dependency-management-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-dependency-management-api-v1-openapi.json
- filename: outsystems-code-quality-api-v1-openapi.json
  format: json
  label: OutSystems ODC Code Quality API
  slug: code-quality-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-code-quality-api-v1-openapi.json
- filename: outsystems-native-application-orchestration-service-api-v1-openapi.json
  format: json
  label: OutSystems ODC Native Mobile Build API
  slug: native-mobile-build-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-native-application-orchestration-service-api-v1-openapi.json
- filename: outsystems-external-library-generation-api-v1-openapi.json
  format: json
  label: OutSystems ODC External Library Generation API
  slug: external-library-generation-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-external-library-generation-api-v1-openapi.json
- filename: outsystems-subscription-api-v1-openapi.json
  format: json
  label: OutSystems ODC Subscription API
  slug: subscription-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/openapi/outsystems-subscription-api-v1-openapi.json
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "azure.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: outsystems.com
  spf: true
hosts:
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: www.outsystems.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: success.outsystems.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Outsystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OutSystems, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: OutSystems
provider_slug: outsystems
slug: outsystems-domain-security
source_filename: outsystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.outsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: false\n- host: success.outsystems.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: outsystems.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"azure.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/outsystems/refs/heads/main/security/outsystems-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Low-Code
- Application Development
- Platform as a Service
- DevOps
- Deployment
- Identity and Access Management
- Artificial Intelligence
- Enterprise Software
- Mobile Development
---
