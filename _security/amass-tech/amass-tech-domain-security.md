---
api_specs:
- filename: amass-tech-cores-biomedcore-api-openapi.yml
  format: yaml
  label: Amass Cores/biomedcore API
  slug: amass-tech-cores-biomedcore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-biomedcore-api-openapi.yml
- filename: amass-tech-cores-drugcore-api-openapi.yml
  format: yaml
  label: Amass Cores/drugcore API
  slug: amass-tech-cores-drugcore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-drugcore-api-openapi.yml
- filename: amass-tech-cores-genecore-api-openapi.yml
  format: yaml
  label: Amass Cores/genecore API
  slug: amass-tech-cores-genecore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-genecore-api-openapi.yml
- filename: amass-tech-cores-patentcore-api-openapi.yml
  format: yaml
  label: Amass Cores/patentcore API
  slug: amass-tech-cores-patentcore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-patentcore-api-openapi.yml
- filename: amass-tech-cores-regulatorycore-api-openapi.yml
  format: yaml
  label: Amass Cores/regulatorycore API
  slug: amass-tech-cores-regulatorycore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-regulatorycore-api-openapi.yml
- filename: amass-tech-cores-trialcore-api-openapi.yml
  format: yaml
  label: Amass Cores/trialcore API
  slug: amass-tech-cores-trialcore-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-cores-trialcore-api-openapi.yml
- filename: amass-tech-credits-api-openapi.yml
  format: yaml
  label: Amass Credits API
  slug: amass-tech-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amass-tech/openapi/amass-tech-credits-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: amass.tech
  spf: true
hosts:
- cert_expires: Jan 30 04:19:49 2027 GMT
  host: amass.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Amass Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amass, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Amass
provider_slug: amass-tech
slug: amass-tech-domain-security
source_filename: amass-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amass.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 04:19:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amass.tech\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/amass-tech/security/amass-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Life Sciences
- Data Intelligence
- MCP
---
