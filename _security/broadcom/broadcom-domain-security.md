---
api_specs:
- filename: broadcom-vsphere-automation-openapi.yml
  format: yaml
  label: Broadcom vSphere Automation API
  slug: vsphere-automation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-vsphere-automation-openapi.yml
- filename: broadcom-operations-for-applications-openapi.yml
  format: yaml
  label: Broadcom Operations for Applications REST API
  slug: operations-for-applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-operations-for-applications-openapi.yml
- filename: broadcom-vmware-cloud-foundation-openapi.yml
  format: yaml
  label: Broadcom VMware Cloud Foundation API
  slug: vmware-cloud-foundation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-vmware-cloud-foundation-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: broadcom.com
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: developer.broadcom.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Broadcom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Broadcom, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Broadcom
provider_slug: broadcom
slug: broadcom-domain-security
source_filename: broadcom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.broadcom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: broadcom.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/security/broadcom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
- Fortune 500
---
