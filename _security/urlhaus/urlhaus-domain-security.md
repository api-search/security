---
description: ''
domains:
- caa:
  - 0 issue "swisssign.com"
  - 0 issue "globalsign.com"
  - 0 issuewild "globalsign.com"
  - 0 issue "pki.goog"
  - 0 issuewild "swisssign.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: abuse.ch
  spf: true
hosts:
- cert_expires: Aug 29 07:08:43 2026 GMT
  host: urlhaus-api.abuse.ch
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urlhaus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for URLhaus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: URLhaus
provider_slug: urlhaus
slug: urlhaus-domain-security
source_filename: urlhaus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: urlhaus-api.abuse.ch\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 07:08:43 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: abuse.ch\n  dnssec: true\n  caa:\n  - 0 issue \"swisssign.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"swisssign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urlhaus/refs/heads/main/security/urlhaus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Anti Malware
- Public APIs
---
