---
api_specs:
- filename: inductive-automation-ignition-gateway.yaml
  format: yaml
  label: Ignition Gateway REST API
  slug: ignition-gateway-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inductive-automation/refs/heads/main/openapi/inductive-automation-ignition-gateway.yaml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: inductiveautomation.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: inductiveautomation.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.docs.inductiveautomation.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inductive Automation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inductive Automation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Inductive Automation
provider_slug: inductive-automation
slug: inductive-automation-domain-security
source_filename: inductive-automation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inductiveautomation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.docs.inductiveautomation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: inductiveautomation.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inductive-automation/refs/heads/main/security/inductive-automation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SCADA
- HMI
- Manufacturing
- IIoT
- Industrial Automation
- Industrial IoT
- OPC UA
---
