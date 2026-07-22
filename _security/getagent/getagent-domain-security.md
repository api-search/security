---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getagent.co.uk
  spf: true
hosts:
- cert_expires: Oct  7 00:31:21 2026 GMT
  host: getagent.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getagent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Getagent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Getagent
provider_slug: getagent
slug: getagent-domain-security
source_filename: getagent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getagent.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:31:21 2026 GMT\n  hsts: null\ndomains:\n- domain: getagent.co.uk\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getagent/refs/heads/main/security/getagent-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- PropTech
- Real Estate
- Estate Agents
- Property
- Comparison
- United Kingdom
---
