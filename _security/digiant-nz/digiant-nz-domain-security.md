---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: digiant.nz
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: a2aregistry.org
  spf: true
hosts:
- host: digiant.nz
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''digiant.nz'''
- cert_expires: Oct 31 19:34:00 2026 GMT
  host: a2aregistry.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 21 21:14:11 2026 GMT
  host: a2a-browser.digiant.nz
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Digiant Nz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for digiantnz, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: digiantnz
provider_slug: digiant-nz
slug: digiant-nz-domain-security
source_filename: digiant-nz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digiant.nz\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''digiant.nz'''\n  hsts: null\n- host: a2aregistry.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 19:34:00 2026 GMT\n  hsts: false\n- host: a2a-browser.digiant.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 21 21:14:11 2026 GMT\n  hsts: null\ndomains:\n- domain: digiant.nz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: a2aregistry.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digiant-nz/refs/heads/main/security/digiant-nz-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- A2A
- Agents
- Web Search
- Web Scraping
- Search
- Micropayments
- Lightning
- New Zealand
---
