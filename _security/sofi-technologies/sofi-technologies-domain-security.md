---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sofi.com
  spf: true
hosts:
- cert_expires: Dec  8 23:40:23 2026 GMT
  host: www.sofi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.sofi.com
  https: false
- cert_expires: Dec  8 23:40:23 2026 GMT
  host: api.sofi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sofi Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoFi Technologies, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SoFi Technologies
provider_slug: sofi-technologies
slug: sofi-technologies-domain-security
source_filename: sofi-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sofi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:40:23 2026 GMT\n  hsts: null\n- host: developer.sofi.com\n  https: false\n- host: api.sofi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:40:23 2026 GMT\n  hsts: null\ndomains:\n- domain: sofi.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/security/sofi-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fintech
- Personal Finance
- Banking
---
