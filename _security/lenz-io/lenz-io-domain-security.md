---
api_specs:
- filename: lenz-io-account-api-openapi.yml
  format: yaml
  label: lenz-io Account API
  slug: lenz-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-account-api-openapi.yml
- filename: lenz-io-ask-api-openapi.yml
  format: yaml
  label: lenz-io Ask API
  slug: lenz-io-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-ask-api-openapi.yml
- filename: lenz-io-assess-api-openapi.yml
  format: yaml
  label: lenz-io Assess API
  slug: lenz-io-assess-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-assess-api-openapi.yml
- filename: lenz-io-citecheck-api-openapi.yml
  format: yaml
  label: lenz-io Citecheck API
  slug: lenz-io-citecheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-citecheck-api-openapi.yml
- filename: lenz-io-discovery-api-openapi.yml
  format: yaml
  label: lenz-io Discovery API
  slug: lenz-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-discovery-api-openapi.yml
- filename: lenz-io-extract-api-openapi.yml
  format: yaml
  label: lenz-io Extract API
  slug: lenz-io-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-extract-api-openapi.yml
- filename: lenz-io-lenz-ai-fact-checking-api-api-openapi.yml
  format: yaml
  label: lenz-io Lenz — AI Fact Checking API
  slug: lenz-io-lenz-ai-fact-checking-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-lenz-ai-fact-checking-api-api-openapi.yml
- filename: lenz-io-library-api-openapi.yml
  format: yaml
  label: lenz-io Library API
  slug: lenz-io-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-library-api-openapi.yml
- filename: lenz-io-review-api-openapi.yml
  format: yaml
  label: lenz-io Review API
  slug: lenz-io-review-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-review-api-openapi.yml
- filename: lenz-io-verifications-api-openapi.yml
  format: yaml
  label: lenz-io Verifications API
  slug: lenz-io-verifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-verifications-api-openapi.yml
- filename: lenz-io-verify-api-openapi.yml
  format: yaml
  label: lenz-io Verify API
  slug: lenz-io-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lenz-io/openapi/lenz-io-verify-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: lenz.io
  spf: true
hosts:
- cert_expires: Jan 27 22:42:03 2027 GMT
  host: lenz.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lenz Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for lenz-io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: lenz-io
provider_slug: lenz-io
slug: lenz-io-domain-security
source_filename: lenz-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lenz.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 22:42:03 2027 GMT\n  hsts: false\ndomains:\n- domain: lenz.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/lenz-io/security/lenz-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Fact-Checking
- Enterprise
- API
- Audit
---
