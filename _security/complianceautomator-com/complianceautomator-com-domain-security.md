---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: complianceautomator.com
  spf: true
hosts:
- cert_expires: Jan 10 13:06:23 2027 GMT
  host: complianceautomator.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ComplianceAutomator Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ComplianceAutomator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ComplianceAutomator
provider_slug: complianceautomator-com
slug: complianceautomator-com-domain-security
source_filename: complianceautomator-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: complianceautomator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 13:06:23 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: complianceautomator.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/complianceautomator-com/security/complianceautomator-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compliance
- Audit Readiness
- SOC 2
- ISO 27001
- HIPAA
- GDPR
- Governance Risk and Compliance
- Software-as-a-Service
---
