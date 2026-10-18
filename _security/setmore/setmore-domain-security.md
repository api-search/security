---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:itsupport@anywhere.co"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: setmore.com
  spf: true
hosts:
- cert_expires: Dec  8 19:45:44 2026 GMT
  host: www.setmore.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Setmore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Setmore, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Setmore
provider_slug: setmore
slug: setmore-domain-security
source_filename: setmore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.setmore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 19:45:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: setmore.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:itsupport@anywhere.co\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/setmore/refs/heads/main/security/setmore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Scheduling
- Software-as-a-Service
- Appointment
- BusinessTools
- Company
---
