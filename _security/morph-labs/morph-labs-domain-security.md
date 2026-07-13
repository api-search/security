---
api_specs:
- filename: morph-labs-openapi.yml
  format: yaml
  label: Morph Apply API
  slug: morph-apply-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morph-labs/refs/heads/main/openapi/morph-labs-openapi.yml
- filename: morph-labs-openapi.yml
  format: yaml
  label: Morph Embeddings API
  slug: morph-embeddings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morph-labs/refs/heads/main/openapi/morph-labs-openapi.yml
- filename: morph-labs-openapi.yml
  format: yaml
  label: Morph Rerank API
  slug: morph-rerank-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/morph-labs/refs/heads/main/openapi/morph-labs-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: morphllm.com
  spf: true
hosts:
- cert_expires: Sep 14 19:39:05 2026 GMT
  host: morphllm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 05:54:49 2026 GMT
  host: docs.morphllm.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 10:12:49 2026 GMT
  host: api.morphllm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morph Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morph, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Morph
provider_slug: morph-labs
slug: morph-labs-domain-security
source_filename: morph-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: morphllm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 19:39:05 2026 GMT\n  hsts: null\n- host: docs.morphllm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 05:54:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.morphllm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:12:49 2026 GMT\n  hsts: null\ndomains:\n- domain: morphllm.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morph-labs/refs/heads/main/security/morph-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Code Editing
- Fast Apply
- Embeddings
- Sandboxes
---
