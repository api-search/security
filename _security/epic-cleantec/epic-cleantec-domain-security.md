---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: epiccleantec.com
  spf: true
hosts:
- cert_expires: Sep 22 00:31:33 2026 GMT
  host: epiccleantec.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epic Cleantec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epic CleanTec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Epic CleanTec
provider_slug: epic-cleantec
slug: epic-cleantec-domain-security
source_filename: epic-cleantec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: epiccleantec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 00:31:33 2026 GMT\n  hsts: false\ndomains:\n- domain: epiccleantec.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epic-cleantec/refs/heads/main/security/epic-cleantec-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Water
- Water Reuse
- Wastewater
- Cleantech
- Sustainability
- Buildings
- Real-Estate
- Climate Tech
- Internet of Things
---
