---
api_specs:
- filename: exoscale-openapi.yml
  format: yaml
  label: Exoscale API
  slug: exoscale
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exoscale/refs/heads/main/openapi/exoscale-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com"
  - 0 iodef "mailto:pki@exoscale.net"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exoscale.com
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: www.exoscale.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: portal.exoscale.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 04:34:22 2026 GMT
  host: openapi-v2.exoscale.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exoscale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exoscale, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Exoscale
provider_slug: exoscale
slug: exoscale-domain-security
source_filename: exoscale-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.exoscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\n- host: portal.exoscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: false\n- host: openapi-v2.exoscale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:34:22 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: exoscale.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com\"\n  - 0 iodef \"mailto:pki@exoscale.net\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exoscale/refs/heads/main/security/exoscale-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Infrastructure
- Compute
- Storage
- Kubernetes
- DBaaS
- Europe
---
