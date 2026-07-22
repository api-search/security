---
description: ''
domains:
- caa:
  - cdn.webflow.com.
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: abbycare.org
  spf: true
hosts:
- cert_expires: Sep 29 17:36:44 2026 GMT
  host: www.abbycare.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abbycare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abbycare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Abbycare
provider_slug: abbycare
slug: abbycare-domain-security
source_filename: abbycare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.abbycare.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 17:36:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: abbycare.org\n  dnssec: true\n  caa:\n  - cdn.webflow.com.\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abbycare/refs/heads/main/security/abbycare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Caregiving
- Home Care
- Medicaid
- Health Tech
- Artificial Intelligence
---
