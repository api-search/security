---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: culinahealth.com
  spf: true
hosts:
- cert_expires: Dec 27 21:08:09 2026 GMT
  host: culinahealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Culina Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Culina Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Culina Health
provider_slug: culina-health
slug: culina-health-domain-security
source_filename: culina-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: culinahealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 21:08:09 2026 GMT\n  hsts: false\ndomains:\n- domain: culinahealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/culina-health/refs/heads/main/security/culina-health-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- Nutrition
- Telehealth
- Dietitian
- VirtualCare
---
