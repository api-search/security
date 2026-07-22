---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: epocrates.com
  spf: true
hosts:
- cert_expires: Aug 22 23:59:59 2026 GMT
  host: www.epocrates.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Epocrates Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Epocrates, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Epocrates
provider_slug: epocrates
slug: epocrates-domain-security
source_filename: epocrates-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.epocrates.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: epocrates.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/epocrates/refs/heads/main/security/epocrates-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Medical Reference
- Drug Database
- Clinical Decision Support
- Drug Interactions
- Mobile App
- athenahealth
---
