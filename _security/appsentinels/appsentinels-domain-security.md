---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: appsentinels.ai
  spf: true
hosts:
- host: appsentinels.ai
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1127)'
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Appsentinels Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppSentinels, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AppSentinels
provider_slug: appsentinels
slug: appsentinels-domain-security
source_filename: appsentinels-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: appsentinels.ai\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1127)'\n  hsts: null\ndomains:\n- domain: appsentinels.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/appsentinels/security/appsentinels-domain-security.yml
summary_line: DMARC
tags:
- Security
- AI
- API
- Monitoring
- Platform
---
