---
api_specs:
- filename: fapd-info-day-api-openapi.yml
  format: yaml
  label: Free Agentic Publication Digester Day API
  slug: fapd-info-day-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fapd-info/openapi/fapd-info-day-api-openapi.yml
- filename: fapd-info-digests-json-api-openapi.yml
  format: yaml
  label: Free Agentic Publication Digester Digests.json API
  slug: fapd-info-digests-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fapd-info/openapi/fapd-info-digests-json-api-openapi.yml
- filename: fapd-info-feed-xml-api-openapi.yml
  format: yaml
  label: Free Agentic Publication Digester Feed.xml API
  slug: fapd-info-feed-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fapd-info/openapi/fapd-info-feed-xml-api-openapi.yml
- filename: fapd-info-free-agentic-publication-digester-static-read-api-api-openapi.yml
  format: yaml
  label: Free Agentic Publication Digester Free Agentic Publication Digester — Static Read API
  slug: fapd-info-free-agentic-publication-digester-static-read-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fapd-info/openapi/fapd-info-free-agentic-publication-digester-static-read-api-api-openapi.yml
- filename: fapd-info-llms-txt-api-openapi.yml
  format: yaml
  label: Free Agentic Publication Digester Llms.txt API
  slug: fapd-info-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fapd-info/openapi/fapd-info-llms-txt-api-openapi.yml
- filename: fapd-info-sources-json-api-openapi.yml
  format: yaml
  label: Free Agentic Publication Digester Sources.json API
  slug: fapd-info-sources-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fapd-info/openapi/fapd-info-sources-json-api-openapi.yml
- filename: fapd-info-today-json-api-openapi.yml
  format: yaml
  label: Free Agentic Publication Digester Today.json API
  slug: fapd-info-today-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fapd-info/openapi/fapd-info-today-json-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org; accounturi=https://acme-staging-v02.api.letsencrypt.org/acme/acct/295381143; validationmethods=http-01"
  - 0 issue "letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/3364094476; validationmethods=http-01"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fapd.info
  spf: false
hosts:
- cert_expires: Dec 28 06:35:48 2026 GMT
  host: fapd.info
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Free Agentic Publication Digester Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Free Agentic Publication Digester, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Free Agentic Publication Digester
provider_slug: fapd-info
slug: fapd-info-domain-security
source_filename: fapd-info-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fapd.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 06:35:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fapd.info\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-staging-v02.api.letsencrypt.org/acme/acct/295381143;\n    validationmethods=http-01\"\n  - 0 issue \"letsencrypt.org; accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/3364094476;\n    validationmethods=http-01\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fapd-info/security/fapd-info-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Data
- Daily Digest
- Open Data
---
