---
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:contact@ceipal.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "godaddy.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ceipal.com
  spf: true
hosts:
- cert_expires: Dec 12 21:31:16 2026 GMT
  host: www.ceipal.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ceipal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CEIPAL, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: CEIPAL
provider_slug: ceipal
slug: ceipal-domain-security
source_filename: ceipal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ceipal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 21:31:16 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ceipal.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:contact@ceipal.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ceipal/refs/heads/main/security/ceipal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Staffing
- Recruiting
- Software-as-a-Service
- Artificial Intelligence
---
