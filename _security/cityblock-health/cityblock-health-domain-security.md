---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cityblock.com
  spf: true
hosts:
- cert_expires: Oct 10 19:07:14 2026 GMT
  host: www.cityblock.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cityblock Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cityblock Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cityblock Health
provider_slug: cityblock-health
slug: cityblock-health-domain-security
source_filename: cityblock-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cityblock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 19:07:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cityblock.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cityblock-health/refs/heads/main/security/cityblock-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Value-Based Care
- Medicaid
- Primary Care
- Mental Health
- Care Coordination
---
