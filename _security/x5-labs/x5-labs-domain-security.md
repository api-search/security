---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: x5labs.com
  spf: true
hosts:
- cert_expires: Jan  8 11:17:59 2027 GMT
  host: x5labs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: X5 Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for X5 Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: X5 Labs
provider_slug: x5-labs
slug: x5-labs-domain-security
source_filename: x5-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: x5labs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 11:17:59 2027 GMT\n  hsts: false\ndomains:\n- domain: x5labs.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/x5-labs/security/x5-labs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- AI
- Governance
- Enterprise
- Automation
---
