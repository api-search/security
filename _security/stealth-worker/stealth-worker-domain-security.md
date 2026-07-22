---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: stealthworker.com
  spf: true
hosts:
- cert_expires: Sep  5 19:45:01 2026 GMT
  host: www.stealthworker.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stealth Worker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stealth Worker, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Stealth Worker
provider_slug: stealth-worker
slug: stealth-worker-domain-security
source_filename: stealth-worker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stealthworker.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:45:01 2026 GMT\n  hsts: false\ndomains:\n- domain: stealthworker.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stealth-worker/refs/heads/main/security/stealth-worker-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Compliance
- Privacy
- Security Staffing
- Consulting
- InfoSec
---
