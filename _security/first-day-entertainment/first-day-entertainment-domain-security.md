---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: firstdayentertainment.net
  spf: true
hosts:
- cert_expires: Sep 25 02:20:04 2026 GMT
  host: www.firstdayentertainment.net
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: First Day Entertainment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for First Day Entertainment, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: First Day Entertainment
provider_slug: first-day-entertainment
slug: first-day-entertainment-domain-security
source_filename: first-day-entertainment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.firstdayentertainment.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 02:20:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: firstdayentertainment.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/first-day-entertainment/refs/heads/main/security/first-day-entertainment-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Games
- Gaming
- Artificial Intelligence
- Entertainment
- Consumer
- Startup
---
