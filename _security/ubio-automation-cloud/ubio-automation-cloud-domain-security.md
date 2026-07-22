---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ubio.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: automationcloud.net
  spf: true
hosts:
- cert_expires: Oct 16 17:33:12 2026 GMT
  host: ubio.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 20:20:23 2026 GMT
  host: api.automationcloud.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 06:23:53 2026 GMT
  host: vault.automationcloud.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ubio Automation Cloud Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UBIO Automation Cloud, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UBIO Automation Cloud
provider_slug: ubio-automation-cloud
slug: ubio-automation-cloud-domain-security
source_filename: ubio-automation-cloud-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ubio.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 17:33:12 2026 GMT\n  hsts: false\n- host: api.automationcloud.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 20:20:23 2026 GMT\n  hsts: null\n- host: vault.automationcloud.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:23:53 2026 GMT\n  hsts: null\ndomains:\n- domain: ubio.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: automationcloud.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ubio-automation-cloud/refs/heads/main/security/ubio-automation-cloud-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Automation
- Web Automation
- RPA
- Travel
- Booking
- Jobs
- Company
---
