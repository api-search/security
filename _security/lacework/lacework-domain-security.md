---
api_specs:
- filename: lacework-api-v2.0.yaml
  format: yaml
  label: Lacework FortiCNAPP API v2
  slug: rest-api-v2
  spec_type: OpenAPI
  url: https://api.lacework.net/api/v2/docs/lacework-api-v2.0.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lacework.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fortinet.com
  spf: false
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.lacework.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  4 23:59:59 2027 GMT
  host: docs.fortinet.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 18:10:27 2026 GMT
  host: youraccount.lacework.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lacework Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lacework FortiCNAPP, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lacework FortiCNAPP
provider_slug: lacework
slug: lacework-domain-security
source_filename: lacework-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lacework.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.fortinet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: youraccount.lacework.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 18:10:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lacework.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fortinet.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lacework/refs/heads/main/security/lacework-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud Security
- CNAPP
- Compliance
- Threat Detection
- Vulnerability Management
- Kubernetes
- Container Security
---
