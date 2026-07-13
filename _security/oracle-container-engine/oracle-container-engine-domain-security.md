---
api_specs:
- filename: oracle-container-engine-openapi.yml
  format: yaml
  label: Oracle Container Engine for Kubernetes
  slug: oracle-container-engine
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-container-engine/refs/heads/main/openapi/oracle-container-engine-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: oracle.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "symantec.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: oraclecloud.com
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: www.oracle.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: containerengine.us-ashburn-1.oci.oraclecloud.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Oracle Container Engine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oracle Container Engine for Kubernetes, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oracle Container Engine for Kubernetes
provider_slug: oracle-container-engine
slug: oracle-container-engine-domain-security
source_filename: oracle-container-engine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.oracle.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: containerengine.us-ashburn-1.oci.oraclecloud.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: oracle.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: oraclecloud.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"symantec.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-container-engine/refs/heads/main/security/oracle-container-engine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Containers
- Kubernetes
- Oracle
- Orchestration
---
