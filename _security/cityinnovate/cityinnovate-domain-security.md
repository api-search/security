---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: authorium.com
  spf: true
hosts:
- cert_expires: Dec 20 13:50:48 2026 GMT
  host: authorium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cityinnovate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cityinnovate, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Cityinnovate
provider_slug: cityinnovate
slug: cityinnovate-domain-security
source_filename: cityinnovate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: authorium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 13:50:48 2026 GMT\n  hsts: false\ndomains:\n- domain: authorium.com\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cityinnovate/refs/heads/main/security/cityinnovate-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- No-code
- AI
- Platform
- Public-benefit
---
