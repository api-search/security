---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: academia.edu
  spf: true
hosts:
- cert_expires: Sep 28 05:31:42 2026 GMT
  host: www.academia.edu
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Academia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Academia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Academia
provider_slug: academia
slug: academia-domain-security
source_filename: academia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.academia.edu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 05:31:42 2026 GMT\n  hsts: null\ndomains:\n- domain: academia.edu\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/academia/refs/heads/main/security/academia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- academic-research
- research-papers
- scholarly-publishing
- higher-education
- open-access
- academic-social-network
- Preprints
- research-discovery
---
