---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: urbanhire.com
  spf: true
hosts:
- cert_expires: Aug 25 22:53:49 2026 GMT
  host: urbanhire.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urbanhire Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UrbanHire, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: UrbanHire
provider_slug: urbanhire
slug: urbanhire-domain-security
source_filename: urbanhire-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urbanhire.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 22:53:49 2026 GMT\n  hsts: null\ndomains:\n- domain: urbanhire.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanhire/refs/heads/main/security/urbanhire-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Recruiting
- Hiring
- Applicant Tracking
- Assessments
- HR Tech
- Indonesia
---
