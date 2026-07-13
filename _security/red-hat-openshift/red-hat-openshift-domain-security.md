---
api_specs:
- filename: red-hat-openshift-api-openapi.yml
  format: yaml
  label: Red Hat OpenShift Container Platform API
  slug: openshift-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/openapi/red-hat-openshift-api-openapi.yml
- filename: openapi
  format: yaml
  label: Red Hat OpenShift Cluster Manager API
  slug: openshift-cluster-manager-api
  spec_type: OpenAPI
  url: https://api.openshift.com/openapi
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:it-cert-admin@redhat.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: redhat.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: false
  dnssec: false
  domain: openshift.com
  spf: true
hosts:
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: www.redhat.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
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
kind: domain-security
layout: security
method: probed
name: Red Hat Openshift Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Red Hat OpenShift, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Red Hat OpenShift
provider_slug: red-hat-openshift
slug: red-hat-openshift-domain-security
source_filename: red-hat-openshift-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.redhat.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.openshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n- host: api.openshift.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 09:27:05 2026 GMT\n  hsts: false\ndomains:\n- domain: redhat.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:it-cert-admin@redhat.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: openshift.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\
  \n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/red-hat-openshift/refs/heads/main/security/red-hat-openshift-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Containers
- Enterprise
- Hybrid Cloud
- Kubernetes
- PaaS
- Red Hat
---
