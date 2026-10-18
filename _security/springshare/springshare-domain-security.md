---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: springshare.com
  spf: true
hosts:
- cert_expires: Jan  1 05:18:51 2027 GMT
  host: springshare.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Springshare Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Springshare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Springshare
provider_slug: springshare
slug: springshare-domain-security
source_filename: springshare-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: springshare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 05:18:51 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: springshare.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/springshare/refs/heads/main/security/springshare-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Library Services
- Software-as-a-Service
- Education
- Open Source
---
