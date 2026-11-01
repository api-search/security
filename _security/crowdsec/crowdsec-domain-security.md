---
api_specs:
- filename: crowdsec-allow-lists-api-openapi.yml
  format: yaml
  label: Crowdsec Allow Lists API
  slug: crowdsec-allow-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-allow-lists-api-openapi.yml
- filename: crowdsec-blocklists-api-openapi.yml
  format: yaml
  label: Crowdsec Blocklists API
  slug: crowdsec-blocklists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-blocklists-api-openapi.yml
- filename: crowdsec-cves-api-openapi.yml
  format: yaml
  label: Crowdsec CVEs API
  slug: crowdsec-cves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-cves-api-openapi.yml
- filename: crowdsec-hub-api-openapi.yml
  format: yaml
  label: Crowdsec Hub API
  slug: crowdsec-hub-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-hub-api-openapi.yml
- filename: crowdsec-info-api-openapi.yml
  format: yaml
  label: Crowdsec Info API
  slug: crowdsec-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-info-api-openapi.yml
- filename: crowdsec-integrations-api-openapi.yml
  format: yaml
  label: Crowdsec Integrations API
  slug: crowdsec-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-integrations-api-openapi.yml
- filename: crowdsec-metrics-api-openapi.yml
  format: yaml
  label: Crowdsec Metrics API
  slug: crowdsec-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crowdsec/openapi/crowdsec-metrics-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crowdsec.net
  spf: true
hosts:
- cert_expires: Dec 30 03:27:28 2026 GMT
  host: www.crowdsec.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Crowdsec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crowdsec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crowdsec
provider_slug: crowdsec
slug: crowdsec-domain-security
source_filename: crowdsec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.crowdsec.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 03:27:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: crowdsec.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/crowdsec/security/crowdsec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Security
- Threat Intelligence
- Open Source
- Community
- Automation
- CrowdSec
---
