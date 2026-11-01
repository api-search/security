---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bonsaihealth.com
  spf: true
hosts:
- cert_expires: Dec 30 15:44:01 2026 GMT
  host: www.bonsaihealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bonsai Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bonsai Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bonsai Health
provider_slug: bonsai-health
slug: bonsai-health-domain-security
source_filename: bonsai-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bonsaihealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 15:44:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bonsaihealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bonsai-health/security/bonsai-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Healthcare
- AI
- PatientEngagement
- Automation
---
