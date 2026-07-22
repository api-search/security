---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: safely.com
  spf: true
hosts:
- cert_expires: Oct 13 13:02:38 2026 GMT
  host: safely.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Safely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Safely, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Safely
provider_slug: safely
slug: safely-domain-security
source_filename: safely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: safely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 13:02:38 2026 GMT\n  hsts: false\ndomains:\n- domain: safely.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safely/refs/heads/main/security/safely-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- InsurTech
- Short-Term Rental
- Vacation Rental
- Guest Screening
- Travel Insurance
- Property Management
---
