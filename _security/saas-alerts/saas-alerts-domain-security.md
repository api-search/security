---
api_specs:
- filename: saas-alerts-openapi.yml
  format: yaml
  label: SaaS Alerts API
  slug: saas-alerts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/saas-alerts/refs/heads/main/openapi/saas-alerts-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: saasalerts.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: kaseya.com
  spf: true
hosts:
- cert_expires: Aug 27 17:01:28 2026 GMT
  host: www.saasalerts.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: help.saasalerts.kaseya.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.saasalerts.com
  https: false
kind: domain-security
layout: security
method: probed
name: Saas Alerts Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SaaS Alerts, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SaaS Alerts
provider_slug: saas-alerts
slug: saas-alerts-domain-security
source_filename: saas-alerts-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saasalerts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 17:01:28 2026 GMT\n  hsts: null\n- host: help.saasalerts.kaseya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\n- host: api.saasalerts.com\n  https: false\ndomains:\n- domain: saasalerts.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kaseya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saas-alerts/refs/heads/main/security/saas-alerts-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- MSP
- SaaS Security
- Security Monitoring
- Threat Detection
- Microsoft 365
- Google Workspace
- MSSP
---
