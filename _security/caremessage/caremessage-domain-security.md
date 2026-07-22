---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: caremessage.org
  spf: true
hosts:
- cert_expires: Sep 12 06:01:41 2026 GMT
  host: www.caremessage.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caremessage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Caremessage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Caremessage
provider_slug: caremessage
slug: caremessage-domain-security
source_filename: caremessage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.caremessage.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:01:41 2026 GMT\n  hsts: false\ndomains:\n- domain: caremessage.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caremessage/refs/heads/main/security/caremessage-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Patient Engagement
- Messaging
- Communications
- Health Equity
- SMS
- Non-Profit
- Digital Health
---
