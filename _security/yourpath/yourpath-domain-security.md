---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yourpathhealth.org
  spf: true
hosts:
- cert_expires: Jan  4 07:40:49 2027 GMT
  host: yourpathhealth.org
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Yourpath Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for YourPath, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: YourPath
provider_slug: yourpath
slug: yourpath-domain-security
source_filename: yourpath-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: yourpathhealth.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 07:40:49 2027 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: yourpathhealth.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yourpath/refs/heads/main/security/yourpath-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Health
- Mental-Health
- Telehealth
- Substance-Use
---
