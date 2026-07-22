---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: stoik.com
  spf: true
hosts:
- cert_expires: Oct  6 17:19:31 2026 GMT
  host: www.stoik.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stoik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stoik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Stoik
provider_slug: stoik
slug: stoik-domain-security
source_filename: stoik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.stoik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 17:19:31 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: stoik.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stoik/refs/heads/main/security/stoik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cyber Insurance
- Cybersecurity
- Insurtech
- Managed Detection and Response
- Email Security
- Phishing Simulation
- Vulnerability Scanning
- Incident Response
- Europe
---
