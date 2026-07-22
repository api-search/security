---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: solace.health
  spf: true
hosts:
- cert_expires: Oct  3 03:01:57 2026 GMT
  host: www.solace.health
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Solace Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Solace Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Solace Health
provider_slug: solace-health
slug: solace-health-domain-security
source_filename: solace-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.solace.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 03:01:57 2026 GMT\n  hsts: false\ndomains:\n- domain: solace.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solace-health/refs/heads/main/security/solace-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Patient Advocacy
- Health Navigation
- Caregiving
- Insurance
- Telehealth
---
