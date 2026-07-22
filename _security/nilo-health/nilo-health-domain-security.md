---
description: ''
domains:
- caa:
  - 0 issue "certainly.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: nilohealth.com
  spf: true
hosts:
- cert_expires: Aug 21 04:02:03 2026 GMT
  host: nilohealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nilo Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nilo Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Nilo Health
provider_slug: nilo-health
slug: nilo-health-domain-security
source_filename: nilo-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nilohealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 04:02:03 2026 GMT\n  hsts: false\ndomains:\n- domain: nilohealth.com\n  dnssec: false\n  caa:\n  - 0 issue \"certainly.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nilo-health/refs/heads/main/security/nilo-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mental Health
- Health
- HR
- Employee Benefits
- Well-being
- Telehealth
- SaaS
---
