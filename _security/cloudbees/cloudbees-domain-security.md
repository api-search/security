---
api_specs:
- filename: cloudbees-unify-openapi.yml
  format: yaml
  label: CloudBees Unify Platform API
  slug: unify
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-unify-openapi.yml
- filename: cloudbees-computer-api-openapi.yml
  format: yaml
  label: CloudBees Computer API
  slug: cloudbees-computer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-computer-api-openapi.yml
- filename: cloudbees-createitem-api-openapi.yml
  format: yaml
  label: CloudBees CreateItem API
  slug: cloudbees-createitem-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-createitem-api-openapi.yml
- filename: cloudbees-job-api-openapi.yml
  format: yaml
  label: CloudBees Job API
  slug: cloudbees-job-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-job-api-openapi.yml
- filename: cloudbees-json-api-openapi.yml
  format: yaml
  label: CloudBees Json API
  slug: cloudbees-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-json-api-openapi.yml
- filename: cloudbees-python-api-openapi.yml
  format: yaml
  label: CloudBees Python API
  slug: cloudbees-python-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-python-api-openapi.yml
- filename: cloudbees-queue-api-openapi.yml
  format: yaml
  label: CloudBees Queue API
  slug: cloudbees-queue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-queue-api-openapi.yml
- filename: cloudbees-xml-api-openapi.yml
  format: yaml
  label: CloudBees Xml API
  slug: cloudbees-xml-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/openapi/cloudbees-xml-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "rapidssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cloudbees.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: cloudbees.io
  note: No SPF TXT record published on the apex; DMARC is p=reject.
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rollout.io
  note: CloudBees Feature Management legacy domain (Rollout). DMARC policy is p=none — monitoring only, not enforcing — where cloudbees.com and cloudbees.io both enforce p=reject.
  spf: true
hosts:
- cert_expires: Nov 15 21:06:49 2026 GMT
  host: www.cloudbees.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 16:52:49 2026 GMT
  host: docs.cloudbees.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: example.cloudbees.com
  https: false
  note: Placeholder host from the CloudBees CI (Jenkins-compatible) specification — CloudBees CI controllers are customer-operated, so there is no CloudBees-run host to probe here.
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: api.cloudbees.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: CloudBees Unify Public API. Unauthenticated GET returns HTTP 401 application/json.
  tls_version: TLSv1.2
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: apidocs.cloudbees.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  note: CloudBees Unify Public API reference; serves the two first-party OpenAPI documents.
  tls_version: TLSv1.2
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: mcp.cloudbees.io
  hsts: false
  hsts_max_age: null
  https: true
  note: CloudBees Unify MCP Server. No HSTS header observed on this host.
  tls_version: TLSv1.2
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: id.cloudbees.io
  hsts: false
  hsts_max_age: null
  https: true
  note: Keycloak authorization server named by the MCP protected-resource document. No HSTS header observed.
  tls_version: TLSv1.2
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: cloudbees.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  note: CloudBees Unify web application (single-page app; answers 200 for every path).
  tls_version: TLSv1.2
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: x-api.rollout.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  note: CloudBees Feature Management REST API edge.
  tls_version: TLSv1.2
hosts_probed: 9
kind: domain-security
layout: security
method: probed
name: Cloudbees Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudBees, probed live across 9 host(s) and 3 registrable domain(s). 8 host(s) serve HTTPS (up to TLSv1.3); 6 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CloudBees
provider_slug: cloudbees
slug: cloudbees-domain-security
source_filename: cloudbees-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts, extended by hand on 2026-09-05 with the cloudbees.io\n  / rollout.io hosts the automated probe did not reach (api, apidocs, mcp and id subdomains, plus the Feature Management\n  edge)\nhosts:\n- host: www.cloudbees.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 21:06:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cloudbees.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 16:52:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: example.cloudbees.com\n  https: false\n  note: Placeholder host from the CloudBees CI (Jenkins-compatible) specification — CloudBees CI controllers are\n    customer-operated, so there is no CloudBees-run host to probe here.\n- host: api.cloudbees.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: CloudBees\
  \ Unify Public API. Unauthenticated GET returns HTTP 401 application/json.\n- host: apidocs.cloudbees.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n  note: CloudBees Unify Public API reference; serves the two first-party OpenAPI documents.\n- host: mcp.cloudbees.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: false\n  hsts_max_age: null\n  note: CloudBees Unify MCP Server. No HSTS header observed on this host.\n- host: id.cloudbees.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: false\n  hsts_max_age: null\n  note: Keycloak authorization server named by the MCP protected-resource document. No HSTS header observed.\n- host: cloudbees.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  note: CloudBees Unify web application (single-page app; answers\
  \ 200 for every path).\n- host: x-api.rollout.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  note: CloudBees Feature Management REST API edge.\ndomains:\n- domain: cloudbees.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"rapidssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: cloudbees.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"sectigo.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n  note: No SPF TXT record published on the apex; DMARC is p=reject.\n- domain: rollout.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  note: CloudBees\
  \ Feature Management legacy domain (Rollout). DMARC policy is p=none — monitoring only, not enforcing\n    — where cloudbees.com and cloudbees.io both enforce p=reject.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudbees/refs/heads/main/security/cloudbees-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CI/CD
- Continuous Delivery
- Continuous Integration
- DevOps
- Feature Flags
- Feature Management
- Jenkins
- Release Orchestration
- Software Delivery
---
