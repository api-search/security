---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: darrow.ai
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:45692213.spf02.hubspotemail.net include:amazonses.com include:_spf.salesforce.com -all
hosts:
- cert_expires: Oct  2 20:17:01 2026 GMT
  host: www.darrow.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  role: marketing site (Webflow)
  tls_version: TLSv1.3
- cert_expires: Sep 26 16:32:07 2026 GMT
  host: auth.darrow.ai
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  role: identity provider (Auth0 tenant)
  tls_version: TLSv1.3
- cert_expires: Sep 25 01:49:39 2026 GMT
  host: portal.darrow.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  role: customer portal entry point
  tls_version: TLSv1.3
- cert_expires: Sep 12 15:11:28 2026 GMT
  host: platform.darrow.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  role: application host
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Darrow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Darrow, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Darrow
provider_slug: darrow
slug: darrow-domain-security
source_filename: darrow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of the darrow.ai marketing, portal, platform and identity hosts\nhosts:\n- host: www.darrow.ai\n  role: marketing site (Webflow)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:17:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: auth.darrow.ai\n  role: identity provider (Auth0 tenant)\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 16:32:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: portal.darrow.ai\n  role: customer portal entry point\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 01:49:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: platform.darrow.ai\n  role: application host\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 15:11:28 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: darrow.ai\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record:\
  \ v=spf1 include:_spf.google.com include:45692213.spf02.hubspotemail.net include:amazonses.com\n    include:_spf.salesforce.com -all\n  dmarc: true\n  dmarc_policy: reject\nobservations:\n- Every host is TLS 1.3 with HSTS; the identity tenant additionally sets includeSubDomains.\n- No CAA record and no DNSSEC on darrow.ai — both are absent, not unprobed.\n- SPF ends in -all and DMARC policy is p=reject, which is a strong published email posture.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/darrow/refs/heads/main/security/darrow-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Legal
- Legal Intelligence
- Litigation
- Artificial Intelligence
- Compliance
- Risk Management
- Insurance
- Data Analytics
---
