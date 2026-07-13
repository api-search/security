---
api_specs:
- filename: ActivitiSwagger-1.4.json
  format: json
  label: Activiti REST API
  slug: activiti-rest-api
  spec_type: OpenAPI
  url: https://github.com/Alfresco/activiti-client-sdk/blob/master/docs/swagger/ActivitiSwagger-1.4.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: activiti.org
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gitbook.io
  spf: true
hosts:
- cert_expires: Sep 26 12:20:20 2026 GMT
  host: www.activiti.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 17:00:10 2026 GMT
  host: activiti.gitbook.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Activiti Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Activiti, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Activiti
provider_slug: activiti
slug: activiti-domain-security
source_filename: activiti-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.activiti.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 12:20:20 2026 GMT\n  hsts: false\n- host: activiti.gitbook.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 17:00:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: activiti.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: gitbook.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activiti/refs/heads/main/security/activiti-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- BPM
- Business Process Management
- Workflow
- BPMN
- Open Source
- Process Automation
- Java
- REST API
---
