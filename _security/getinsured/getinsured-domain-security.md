---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: getinsured.com
  spf: true
hosts:
- cert_expires: Sep 30 22:03:44 2026 GMT
  host: www.getinsured.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getinsured Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetInsured, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: GetInsured
provider_slug: getinsured
slug: getinsured-domain-security
source_filename: getinsured-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getinsured.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 22:03:44 2026 GMT\n  hsts: false\ndomains:\n- domain: getinsured.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getinsured/refs/heads/main/security/getinsured-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Health Insurance
- Government
- Insurance
- Marketplace
- ACA
- SaaS
- Enrollment
---
