---
api_specs:
- filename: swagger.json
  format: json
  label: OpenShift REST API
  slug: openshift-rest-api
  spec_type: OpenAPI
  url: https://api.openshift.com/api/swagger.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: openshift.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: docs.openshift.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 09:27:05 2026 GMT
  host: api.openshift.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: oauth-openshift.apps.openshift.com
  https: false
kind: domain-security
layout: security
method: probed
name: Openshift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenShift, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenShift
provider_slug: openshift
slug: openshift-domain-security
source_filename: openshift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.openshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n- host: api.openshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 09:27:05 2026 GMT\n  hsts: false\n- host: oauth-openshift.apps.openshift.com\n  https: false\ndomains:\n- domain: openshift.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openshift/refs/heads/main/security/openshift-domain-security.yml
summary_line: TLSv1.3
tags:
- CI/CD
- Cloud Native
- Containers
- DevOps
- Enterprise
- Kubernetes
- PaaS
---
