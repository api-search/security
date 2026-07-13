---
api_specs:
- filename: semantic-scholar-academic-graph-openapi.yml
  format: yaml
  label: Semantic Scholar Academic Graph API
  slug: semantic-scholar-academic-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semantic-scholar/refs/heads/main/openapi/semantic-scholar-academic-graph-openapi.yml
- filename: semantic-scholar-recommendations-openapi.yml
  format: yaml
  label: Semantic Scholar Recommendations API
  slug: semantic-scholar-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semantic-scholar/refs/heads/main/openapi/semantic-scholar-recommendations-openapi.yml
- filename: semantic-scholar-datasets-openapi.yml
  format: yaml
  label: Semantic Scholar Datasets API
  slug: semantic-scholar-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semantic-scholar/refs/heads/main/openapi/semantic-scholar-datasets-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: semanticscholar.org
  spf: true
hosts:
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: www.semanticscholar.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  4 23:59:59 2027 GMT
  host: api.semanticscholar.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Semantic Scholar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Semantic Scholar, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Semantic Scholar
provider_slug: semantic-scholar
slug: semantic-scholar-domain-security
source_filename: semantic-scholar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.semanticscholar.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: false\n- host: api.semanticscholar.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: semanticscholar.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semantic-scholar/refs/heads/main/security/semantic-scholar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Academic
- Research
- Papers
- Citations
- Authors
- Scientific Literature
- AI
- Recommendations
---
